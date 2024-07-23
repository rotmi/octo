# Finetune Octo on Amazon SageMaker

The Jupyter notebook [octo-sagemaker.ipynb](https://github.com/rotmi/octo/blob/main/octo-sagemaker.ipynb) provides you a simple example how to finetune the Octo robotics model on Amazon SageMaker using a slightly adapted finetuning script that Octo provides. For additional details on Octo have a look into the upstream [Octo repo](https://github.com/octo-models/octo)

The notebook has been tested successfully on an Amazon SageMaker Studio ml.t3.medium instance running an Amazon Sagemaker Distribution 1.9 image.

Your execution environment / AWS config chain for the notebook needs to have:
- Sufficient IAM permissions e.g. Amazon S3, Amazon SageMaker, Amazon CloudWatch
- Amazon SageMaker instance quotas in place for the training job


TODO:
- wandb integration is currently disabled within the finetuning script
- The trained model within the training container is currently not postprocessed/packaged by the finetuning script and not put into /opt/ml/model for upload to S3 by Amazon SageMaker

