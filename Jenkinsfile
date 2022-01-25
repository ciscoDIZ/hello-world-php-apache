pipeline{
    agent any
    stages {
        
        stage("Build") {
            steps {
                sh "docker build -t hello-word-php-apache ."        
            }
        }
        stage("Run") {
            steps {
                sh "docker run -d -rm -p 8085:80 hello-word-php-apache"
            }
        }
        
    }

}