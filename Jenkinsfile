#!/usr/bin/env groovy

pipeline {
    agent any
    options {
        timestamps()
    }
    stages {
<<<<<<< HEAD
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
        stage('Test') {
            steps {
                echo("Testing project for ")
                sleep(time:5,unit:'SECONDS')
                sh 'mvn test'
            }
            post {
                success {
                    echo("Test stage completed with result 'SUCCESS'.")
                }
                failure {
                    echo("Test stage completed with result 'FAILURE'.")
                }
            }
        }
        stage('Deploy') {
            steps {
                echo("Deploying project for ")
                sleep(time:5,unit:'SECONDS')
                sh 'mvn deploy'
            }
            post {
                success {
                    echo("Deploy stage completed with result 'SUCCESS'.")
                }
                failure {
                    echo("Deploy stage completed with result 'FAILURE'.")
                }
            }
        }
    }
    post {
        success {
            echo("Pipeline completed for  with result 'SUCCESS'.")
        }
        failure {
            echo("Pipeline completed for  with result 'FAILURE'.")
        }
=======

        stage('clean') {

            steps {

                echo("Building project for me")

                sleep(time:5,unit:'SECONDS')

		            sh 'mvn clean'

            }

            post {

                success {

                    echo("Clean stage completed with result 'SUCCESS'.")

                }

                failure {

                    echo("Clean stage completed with result 'FAILURE'.")

                }

            }

        }

        stage('package') {

            steps {

                echo("Testing project for me")

                sleep(time:5,unit:'SECONDS')

		            sh 'mvn package'

            }

            post {

                success {

                    echo("package stage completed with result 'SUCCESS'.")

                }

                failure {

                    echo("package stage completed with result 'FAILURE'.")

                }

            }

        }

    }

    post {

        success {

            echo("Pipeline completed for me with result 'SUCCESS'.")

        }

        failure {

            echo("Pipeline completed for me with result 'FAILURE'.")

        }

>>>>>>> 73df4c17a7b708b34bc5ca4697b445e8e3a4077f
    }
}
