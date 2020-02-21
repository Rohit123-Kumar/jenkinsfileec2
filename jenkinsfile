pipeline {
    agent any
    stages {
        stage ('clone repo') {
            steps {
                sh "export AWS_DEFAULT_REGION=ap-south-1"
                sh "aws cloudformation create-stack --stack-name demostack --template-body file://ec2cf.json --region 'ap-south-1'"
            }
        }
    }
}
