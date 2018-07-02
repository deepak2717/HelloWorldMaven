pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'mvn clean compile'
            }
        }
        stage('Test'){
            steps {
                sh 'mvn test'

            }
        }
        stage('Deploy') {
            steps {
                sh 'mvn deploy'

            }
        }
    }
}
