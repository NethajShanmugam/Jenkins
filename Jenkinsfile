pipeline {
    agent any 

    stages {
        stage ('complile stage') {

            steps{
                withMaven(maven : 'Maven_3_9_5') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('test stage') {

            steps{
                withMaven(maven : 'Maven_3_9_5') {
                    sh 'mvn test'
                }
            }
        }

        stage ('Deploy stage') {

            steps{
                withMaven(maven : 'Maven_3_9_5') {
                    sh 'mvn deploy'
                }
            }
        }

    }
}
