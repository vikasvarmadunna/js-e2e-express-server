pipeline{
    agent any
    stages{
        stage('vcs'){
            steps{
               git url: 'https://github.com/vikasvarmadunna/js-e2e-express-server.git', branch: 'amazon'
                 }
        }
    
        
        stage('build'){
            steps{
                agent { label 'jdk-11-mvn' }
                sh 'npm install'
     		sh 'npm run build'
                 }
        }

        
    }     
}
