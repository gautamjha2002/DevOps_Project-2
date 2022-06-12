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

        stage('Deploy on tesing Server'){
            steps{
                echo "Deployed on Testing Server"

            }
        }

        stage('deploy on Production server'){
            steps{
               echo "Deplloyed on Production server"
                
            }
        }
    }
}