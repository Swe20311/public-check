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
                sh "echo hi"
            }
        }
        stage('archive artifacts'){
            steps{
                archiveArtifacts artifacts: '*'
            }
        }
    }
}
