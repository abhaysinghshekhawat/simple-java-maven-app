pipeline{
    agent any
    stages{
        stage('gitscm'){
            steps{
                echo 'github'
                git 'https://github.com/vimallinuxworld13/simple-java-maven-app.git'
                sh 'mvn package'
                sh 'java -jar target/*.jar'
                archiveArtifacts artifacts: 'target/*.jar', followSymlinks: false
            }
            }
        }
    }
