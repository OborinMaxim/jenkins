pipeline {
    agent { docker 'aragast/agent:7' }
    stages {
        stage('Declarative Pipeline') {
            steps {
                git clone https://github.com/aragastmatb/example-playbook.git
                ansible-playbook site.yml -i inventory/prod.yml
            }
        }
    }
}
