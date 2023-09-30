pipeline
{
    agent{
        node {label 'workstation'}
    }

    stages{
        stage('Build'){
            steps{
             echo 'Unit tests'
            }
        }

        stage('Unit tests'){
            steps{
             echo 'Unit tests'
            }
        }

        stage('Code Analysis'){
            steps{
             sh 'sonar-scanner -Dsonar.host.url=http://172.31.20.113:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=dispatch'
            }
        }

        stage('Security Scans'){
            steps{
             echo 'Security Scans'
            }
        }

        stage('Publish a Artifact'){
            steps{
             echo 'Publish a Artifact'
            }
        }

    }
}