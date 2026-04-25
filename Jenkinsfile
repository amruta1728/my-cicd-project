pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/amruta1728/my-cicd-project.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                cd ansible
                ansible-playbook -i inventory deploy.yml
                '''
            }
        }
    }
}
