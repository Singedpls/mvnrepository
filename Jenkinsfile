pipeline {
    agent any   //any nodes 

    stages {
        stage('Build App') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Test') {
            steps {
                echo 'Test Maven Build'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }
    post{
        always{
            emailext body: 'Error en Build', subject: 'Pipeline Status', to: 'alumno@gmail.com'   
        }
    }
}
