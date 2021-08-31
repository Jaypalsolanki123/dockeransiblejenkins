pipeline{
    agent any

    stages{
        stage('SCM Checkout'){
            steps{
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/Jaypalsolanki123/JenkinsDemo'
            }
        }    
        stage('Maven Build'){
            steps{
                sh "mvn clean package"
            }
        }
    }
}
