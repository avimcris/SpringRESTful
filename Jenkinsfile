pipeline {
    
    agent any
    tools {maven "mavenV2"}
    stages{
        
        stage("checkout"){
            steps{
                git branch: "main", url: "https://github.com/avimcris/SpringRESTful.git"
            }
        }
        
        stage("build"){
            steps{
                sh "mvn compile"
            }
        }
        
        stage("test"){
            steps{
                sh "mvn test"
            }
        }
    }
}
