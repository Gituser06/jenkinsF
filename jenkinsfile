


pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                #echo 'Building..'
		withMaven(maven: 'MAVEN_HOME'){
			sh 'mvn test'
		}
            }
        }
        stage('Test') {
            steps {
               # echo 'Testing..'
		withMaven(maven: 'MAVEN_HOME'){
                        sh 'mvn test'
		}
            }
        }
        stage('Deploy') {
            steps {
                #echo 'Deploying....'
		withMaven(maven: 'MAVEN_HOME'){
                        sh 'mvn test'
		}
            }
        }
    }
}
