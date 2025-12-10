pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'master', url: 'https://github.com/amruta1728/my-cicd-project.git'
            }
        }

        stage('Run Ansible Playbook') {
            steps {
                sh '''
                ansible-playbook -i inventory.ini deploy.yml
                '''
            }
        }
    }

    post {
        success {
            echo "Deployment completed successfully!"
        }
        failure {
            echo "Deployment failed. Check logs."
        }
    }
}
