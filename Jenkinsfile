pipeline {
    agent any
    stages {
        stage('Upload to AWS') {
            steps {
                withAWS(profile:'aws-static') {
                    s3Upload(file:'index.html', bucket:'ruiqinng-devops-project3-jenkins-pipeline', path:'index.html')
                }
            }
        }
    }
}