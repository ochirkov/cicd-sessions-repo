pipeline {
    
    agent any

    options {
        timestamps ()
    }

    stages {
        
        stage('Checkout Stage') {
            steps {
                git branch: 'main',
                url: 'https://github.com/ochirkov/cicd-sessions-repo.git'
            }
        }

        stage('Docs Stage') {
            steps {
                sh "ls -l"
                sh "tox -e docs"
            }
        }        
    }
}
