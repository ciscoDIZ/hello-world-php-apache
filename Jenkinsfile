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
                sh "docker run -p 80:80 hello-word-php-apache"
            }
        }
        stage("Clone") {
            steps{
                sh "git clone github.com/ciscoDIZ/php-pipeline.git repository"
            }
        }
    }

}