pipeline {
    agent any
    stages {
        stage('Declarative Pipeline') {
            steps {
                sh 'rm -r *'                
                sh 'git clone https://github.com/OborinMaxim/jenkins.git'
                sh 'ansible-playbook jenkins/site.yml -i jenkins/inventory/prod.yml'
            }
        }
    }
}
