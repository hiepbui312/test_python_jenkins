pipeline {
    agent { 
        node {
            label 'hiepbui'
            }
      }
    triggers {
        pollSCM 'H/10 * * * *'
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh "docker compose ps"
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                echo "doing test stuff.."
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff.."
                '''
            }
        }
    }
}
