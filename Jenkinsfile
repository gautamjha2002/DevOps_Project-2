pipeline{
    agent any
    stages{
        stage('building Application'){
            steps{
                sh 'mvn -f  pom.xml clean package'
            }
            
        }
    }
}