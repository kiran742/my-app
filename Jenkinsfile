pipeline{
    agent any 
    stages{
        stage('Git checkout'){
            steps{
              git credentialsId: 'githud_cred', url: 'https://github.com/kiran742/my-app.git'
            }
        }
        stage('mvn build'){
            steps{
            sh 'mvn clean package'
            }
        }
            
    }
}
