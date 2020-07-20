pipeline {
    /* insert Declarative Pipeline here */
    agent any
        stages {
        stage('Deploy/Build App') {
            steps {
                sh '''
                    echo 'Application deployed successfully!'
                '''
            }
        }
        stage('Frontend tests') {
            steps {
                sh '''
                    cd frontend-project-cypress/cypress-demo3-vue-project/rasi10-hotel-test-vue/ 
                    npm install && npm run cypress:run
                    echo 'Need to publish test results'
                    pwd
                    ls -lart
                '''
            }
        }
        
        stage('Backend tests') {
            steps {

                sh 'pwd'
                sh 'ls -lart'
            }
        }
        
        stage('Performance tests') {
            steps {
                sh 'pwd'
                sh 'ls -lart'
            }
        }
        
    }
}