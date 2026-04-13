pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compile and package the source code into a deployable artifact.'
                echo 'Tool: Maven - automates compilation, dependency management, and packaging.'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Run unit tests to verify individual components and integration tests to verify component interactions.'
                echo 'Tool: JUnit for unit testing, Selenium for integration testing.'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analyse source code for bugs, code smells, and ensure it meets industry coding standards.'
                echo 'Tool: SonarQube - performs static code analysis and enforces quality gates.'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scan the code and dependencies for known vulnerabilities and CVEs.'
                echo 'Tool: OWASP Dependency-Check - identifies vulnerable third-party libraries.'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploy the packaged application to a staging server that mirrors production.'
                echo 'Tool: AWS CLI - used to deploy application to an AWS EC2 staging instance.'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Run integration tests on the staging environment to validate end-to-end functionality.'
                echo 'Tool: Selenium - automates browser-based integration testing on the staging server.'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploy the verified application to the live production server.'
                echo 'Tool: AWS CLI - deploys the final artifact to an AWS EC2 production instance.'
            }
        }
    }
}
