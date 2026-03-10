pipeline {
    agent any

    stages {

        stage(' GitHub Repository clone') {
            steps {
                git url: 'https://github.com/Premsagar200401/ansibleproject.git',
                branch: 'main'
            }
        }

        stage('Execute Ansible Playbook') {
            steps {
                sh '''
                sudo -u ansible ansible-playbook -i inventory install_nginx.yml
                '''
            }
        }

    }
}
