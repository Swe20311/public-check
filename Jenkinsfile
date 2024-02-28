pipeline{
    agent any
    environment{
        swe="hi there"
    }
    stages{
        stage('git checkout'){
            steps{
                sh "echo $swe"
                sh "ls -la"
            }
        }
        stage('archive artifacts'){
            steps{
                archiveArtifacts artifacts: '*'
            }
        }
    }
}
