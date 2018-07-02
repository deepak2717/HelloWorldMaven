pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps {
	        #withMaven(maven : 'maven_3_3_9') {
                sh 'mvn clean compile'
		#}
            }
        }
        stage('Test'){
            steps {
	        #withMaven(maven : 'maven_3_3_9') {
                sh 'mvn test'
                #}

            }
        }
        stage('Deploy') {
            steps {
                #withMaven(maven : 'maven_3_3_9') {
                sh 'mvn deploy'
                #}

            }
        }
    }
}
