pipeline {
    agent any
    environment {
        registryURI = "registry.hub.docker.com/"
        registry = "prakuldip/jenkinsfile_kul_app_trialone"
        registryCredential = "dockerhub_cred"
    }
stages {
        stage('docker image build,push to remote and delete locally') {
            steps{
                script {
                  sh 'terraform init'
                    }
                   
                }
            }
        }
    post { 
        always { 
            echo 'Deleting Workspace'
            deleteDir() /* clean up our workspace */
        }
    }
}