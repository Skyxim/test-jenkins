pipeline {
    agent none
    stages {
        stage('mysql'){
            agent{
                image "mysql:5.7.37-oracle"
            }
            steps{
            sh 'echo "run mysql"'
            }
        }
        stage('redis'){
            agent{
                image "redis:5.0.14-bullseye"
            }
            steps{
                sh 'echo "run redis"'
            }
        }

    }

}
