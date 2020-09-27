pipeline {
    agent any
    stages {
        stage('gitebay') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'manojthirumani-git', url: 'https://github.com/manojthirumani/ebay.git']]])
            }
        }
        stage('checkout') {
            steps {
            echo 'checkout project'    
                } }
                stage('build') {
            steps {
            echo 'buliding project'
                } }
                stage('test') {
            steps {
            echo 'testing project'
                } }
                stage('QA Deploy') {
            steps {
            echo 'QA Deploy project'
                } }
                stage('prod deploy') {
            steps {
            echo 'prod deploy project'
                } }
           }
        }

