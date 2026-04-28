pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compiling and packaging the code'
                echo 'Tool: Maven'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Running unit tests and integration tests'
                echo 'Tools: JUnit for unit tests, TestNG for integration tests'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analysing code quality against industry standards'
                echo 'Tool: SonarQube'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scanning for known vulnerabilities in dependencies'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploying application to AWS EC2 staging instance'
                echo 'Tool: AWS CLI'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Running integration tests on staging environment'
                echo 'Tool: Selenium'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploying application to AWS EC2 production instance'
                echo 'Tool: AWS CLI'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
