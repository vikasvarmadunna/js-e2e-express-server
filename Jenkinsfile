pipeline{
agent { label 'jdk-11-mvn' }
triggers { pollSCM('* * * * *') }
stages{
stage('vcs'){
steps{
git branch: "main", url: 'https://github.com/vikasvarmadunna/js-e2e-express-server.git'
}
}
stage('build'){
steps{
agent { label 'jdk-11-mvn' }
sh "/usr/bin/npm npm install"
sh "/usr/bin/npm npm run build"

}
}

}     
}
