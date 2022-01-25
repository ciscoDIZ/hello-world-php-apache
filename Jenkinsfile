pipeline{
    agent any
    stages {
        stage("Clone") {
            steps{
                sh "git clone github.com/ciscoDIZ/php-pipeline.git "
            }
        }
        stage("Build") {
            steps {
                sh "sudo docker build -t hello-word-php-apache ."        
            }
        }
        stage("Run") {
            steps {
                sh "sudo docker run -p 80:80 hello-word-php-apache"
            }
        }
    }

}