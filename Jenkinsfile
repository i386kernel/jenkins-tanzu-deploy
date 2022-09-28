pipeline {
    stages {
    // Test Tanzu
       stage("Test Tanzu"){
       agent {
            label 'tanzu-mgmt'
       }
       steps{
            sh 'tanzu cluster list --include-management-cluster'
            sh 'tanzu cluster create -f wk-dev-01.yml'
           }
       }
    }
}

