pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    
    stages {
        
        stage ('clone') {
            steps {
                git url: 'https://github.com/AmithDevOps7907/sparkjava-war.git', branch: 'main'
            }
        }
        stage ('build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

