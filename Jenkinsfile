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
                sh "docker run -p 8095:80 hello-word-php-apache"
            }
        }
        
    }

}