pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                git branch: 'main', url: 'https://github.com/jelenakozemjakina/AnsibleLabs.git'
                sh 'ansible-playbook playbook.yaml --extra-vars "text=$text"'
            }
        }
    }
}
