pipeline{
	agent any
	properties([parameters([string(defaultValue: 'bucketname345', description: 'Select a unique name bucket name', name: 'Bucket', trim: false)])])
	stages{
	stage('Clone Repo') {
	echo "pulling changes from bucket ${params.bucketname345}"
	git url:'https://github.com/aniruddhaparte61/S3cft.git',bucketname345:${params.bucketname345}
	}
	}
}
