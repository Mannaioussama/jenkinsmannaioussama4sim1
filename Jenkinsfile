pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Mannaioussama/jenkinsmannaioussama4sim1.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                sh "mvn clean install -DskipTests"
            }
        }
    }
}
