pipeline {
    agent any

    stages {

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
