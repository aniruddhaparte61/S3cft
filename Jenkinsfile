pipeline{
	agent any
	parameters {
	string(name: 'S3Name',
		defaultValue:'None',
		description: 'Do the funky chicken!') 
	}
	stages{
	stage('Clone Repo') {
		steps {
			sh "export AWS_DEFAULT_REGION=us-east-1"
			sh "aws cloudformation create-stack --stack-name Group87stack --template-body file://s3anicft.json --region 'us-east-1'"
			}
	}
		stage('Test'){
			steps{
				sh "ls"
			}
		}
		stage('Deploy'){
			steps{
				sh "ls"
			}
		}
	
	}
}
