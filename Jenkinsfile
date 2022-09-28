pipeline{
agent { label 'jdk-11-mvn' }
stages{
stage('vcs')
{
steps{
git branch: 'amazon', url: 'https://github.com/vikasvarmadunna/js-e2e-express-server.git'
     }
} 
stage('build'){
  steps{
    sh "npm install" 
    sh "npm run build"
       }
}

     }

}  
