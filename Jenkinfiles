pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application and packaging it into a deployable artefact.'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Running unit tests to verify individual components behave as expected.'
                echo 'Running integration tests to verify the components work together.'
                echo 'Tools: JUnit for unit tests, Selenium for integration tests'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Analysing the source code against industry coding standards.'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Scanning the code and its dependencies for known vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploying the packaged application to the staging server.'
                echo 'Target: AWS EC2 staging instance'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Running integration tests on staging to confirm the application behaves correctly in a production-like environment.'
                echo 'Tool: Selenium'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploying the application to the production server.'
                echo 'Target: AWS EC2 production instance'
            }
        }
    }
}
