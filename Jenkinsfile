pipeline {
    agent { 
        node {
            label 'docker-agent-local'
            }
    }
    triggers {
        githubPush()
    }
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh '''
                echo "Step 1 : build with Jenkinsfile with github webhook"
                '''
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh '''
                echo "Step 2 : test with Jenkinsfile with github webhook"
                '''
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                echo "doing delivery stuff with Jenkinsfile with github webhook"
                '''
            }
        }
    }
}