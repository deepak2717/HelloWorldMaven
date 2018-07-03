pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps {
                maven(maven : 'Maven_3.3.9'){
                        bat "mvn clean compile"
                }
            }
        }
        stage('Test'){
            steps {
                maven(maven : 'Maven_3.3.9'){
                        bat "mvn test"
                }

            }
        }
        stage('Deploy') {
            steps {
               maven(maven : 'Maven_3.3.9'){
                        bat "mvn deploy"
                }

            }
        }
    }
}
