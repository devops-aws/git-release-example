#!/usr/bin/env groovy

pipeline {
    agent any
    options {
        timestamps()
    }
    stages {
        stage('Clean') {
            steps {
                echo("Building project for ")
                sleep(time:5,unit:'SECONDS')
                sh 'mvn clean'
            }
            post {
                success {
                    echo("Build stage completed with result 'SUCCESS'.")
                }
                failure {
                    echo("Build stage completed with result 'FAILURE'.")
                }
            }
        }
}
