pipeline {
    agent any
   
    stages{
        stage("checkout:git") {
            git branch: "master", url: "https://github.com/eduardofarantes/jenkins.git"
        }

        stage("Build:Maven") { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}