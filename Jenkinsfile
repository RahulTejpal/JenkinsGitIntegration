pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/RahulTejpal/JenkinsGitIntegration.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x HelloWorld.java"
                sh "javac HelloWorld.java"
                sh "java HelloWorld"
            }
        }
     stage('Test Code') {
            steps {
                echo "Testing Phase"
            }
        }
    } 
}
