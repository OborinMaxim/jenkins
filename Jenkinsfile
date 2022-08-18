pipeline {
    agent any
    stages {
        stage('Declarative Pipeline') {
            steps {
                sh 'rm -r *'                
                sh 'git clone https://github.com/aragastmatb/example-playbook.git'
                sh 'ansible-playbook example-playbook/site.yml -i example-playbook/inventory/prod.yml'
            }
        }
    }
}
