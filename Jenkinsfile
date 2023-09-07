pipeline {
    agent any

    stages {
        stage("Build") {
            steps {
                
                echo "Building the code project"
            }
            post {
                always {
                    mail to: "newtaltar@gmail.com",
                        subject: "Build Status Email",
                        body: "Build Successfull!"
                }
            }
        }

        stage("Unit and Integration Tests") {
            steps {
                echo "Running unit and integration tests using Marvern..."
            }
        }

        stage("Code Analysis") {
            steps {
                echo "Analyzing code with Sonacube..."
            }
        }

        stage("Security Scan") {
            steps {
                echo "Performing security scan right now..."
            }
        }

        stage("Deploy to Staging") {
            steps {
                echo "Deploying to staging server with AWS"
            }
        }

        stage("Integration Tests on Staging") {
            steps {
                echo "Running integration tests on staging environment like AWS"
            }
        }

        stage("Deploy to Production") {
            steps {
                echo "Deploying to production server with AWS..."
            }
        }
    }
}
