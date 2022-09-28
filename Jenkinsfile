pipeline {
    agent any
    stages {
    // Test Tanzu
       stage("Create Tanzu Workload Cluster"){
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

