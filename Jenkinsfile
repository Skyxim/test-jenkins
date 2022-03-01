pipeline {
    agent none
    stages {
        stage('mysql'){
            agent{
              docker{  image "mysql:5.7.37-oracle"}
            }
            steps{
            sh 'echo "run mysql"'
            }
        }
        stage('redis'){
            agent{
                docker{  image "redis:5.0.14-bullseye"}
            }
            steps{
                sh 'echo "run redis"'
            }
        }
        stage('output'){
            agent none
            steps{
                echo $(docker ps)
            }
        }
    }
}
