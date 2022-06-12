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
               // build job: 'Deploy on Testing Server'
               echo "deploy on testing"

            }
        }

        stage('deploy on Production server'){
            steps{
                // timeout(time:5, unit:'DAYS'){
                //     input message: 'Approve Production Deployment?'
                // }
                // build job: 'Deploy on Production Server'
                echo "deploy to prod"
            }
        }
    }
}