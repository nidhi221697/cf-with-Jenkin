pipeline {
    agent any
    stages {
        stage('Submit stack') {
            steps {
                sh "aws cloudformation create-stack --stack-name ELB-TF --template-body file://ec2-vpc-ALB-tg-SSMParameter.yml --region 'ap-south-1'"
            }
        }
    }
}
