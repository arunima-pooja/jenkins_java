pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/arunima-pooja/jenkins_java.git'
            }
        }

        stage('Compile') {
            steps {
                sh "javac Hello.java"
            }
        }
 
	stage('Run') {
	    steps {
		sh "java Hello"
	    }
	}
   }
}
