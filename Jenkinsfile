pipeline {
    agent any
    stages {
        stage('Build') {
            environment {
                JAVA_HOME = tool('jdk-17')
            }
            steps {
                sh 'mvn clean install -Dmaven.test.skip=true'
                sh './mvnw clean package'
            }
        }
    }
}
