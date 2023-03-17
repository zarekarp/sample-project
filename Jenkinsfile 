pipeline {
    agent any
    stages {
        stage('Build') {
            environment {
                JAVA_HOME = tool('jdk-17')
            }
            steps {
                sh './mvnww clean package'
            }
        }
    }
}
