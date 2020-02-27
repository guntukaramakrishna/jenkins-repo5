pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Get Upstream') {
            steps {
                build(
                    job: "guntukaramakrishna/jenkins-repo4/master",
                    wait: false,
                    propagate: false
                  )
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
