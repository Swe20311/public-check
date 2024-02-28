pipeline{
    agent any
    environment{
        swe="hi there"
    }
    stages{
        stage('git checkout'){
            steps{
            // checkout scmGit(branches: [[name: 'main']], extensions: [], userRemoteConfigs: [[credentialsId: 'swe_git', url: 'https://github.com/Swe20311/dummy.git']])
            //checkout ([$class:'GitSCM',branches: [[name: 'main']],userRemoteConfigs: [[credentialsId: 'swe_git',url: 'https://github.com/Swe20311/dummy.git']]])
                sh "echo $swe"
                sh "ls -la "
            }
        }
        stage('archive artifacts'){
            steps{
                archiveArtifacts artifacts: '*'
            }
        }
    }
}
