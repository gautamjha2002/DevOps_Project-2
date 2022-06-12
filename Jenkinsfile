pipeline{
    agent any
    stages{
        stage('building Application'){
            steps{
                sh 'mvn -f  pom.xml clean package'
            }
            post {
                success {
                    echo "Now Archiving the Artifacts...."
                    archiveArtifacts artifacts: '**/*.war'
                }
            }
            
        }
    }
}