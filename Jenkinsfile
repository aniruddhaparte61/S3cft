pipeline{
	agent any
	stages{
	stage('Clone Repo') {
		steps {
			sh "export AWS_DEFAULT_REGION=us-east-1"
			sh "aws cloudformation create-stack --stack-name ${params.Stackname} --template-body file://s3anicft.json --region 'us-east-1' --parameters ParameterKey='BucketName',ParameterValue=${params.Bucketname}" 
			}
	}
	}
}
