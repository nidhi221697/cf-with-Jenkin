pipeline {
    agent any
    stages {
        stage('Submit stack') {
            steps {
                sh "aws cloudformation create-stack --stack-name s3bucket --template-body file://ec2-vpc-ALB-tg.yml --region 'ap-south-1'"
            }
        }
    }
}
