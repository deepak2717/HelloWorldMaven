pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps {
                maven(maven : 'Maven_3.5.2'){
                        bat "mvn clean compile"
                }
            }
        }
        stage('Test'){
            steps {
                maven(maven : 'Maven_3.5.2'){
                        bat "mvn test"
                }

            }
        }
        stage('Deploy') {
            steps {
               maven(maven : 'Maven_3.5.2'){
                        bat "mvn deploy"
                }

            }
        }
    }
}
