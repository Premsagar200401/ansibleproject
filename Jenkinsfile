pipeline {
    agent any

    stages {

        stage('Execute Ansible Playbook') {
            steps {
                sh '''
                sudo -u ansible ansible-playbook -i inventory install_nginx.yml
                '''
            }
        }

    }
}
