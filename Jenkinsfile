pipeline {
    agent {
        node {
            label 'dist'
        }
    }
    options {
        timestamps()
        timeout(time: 5, unit: 'MINUTES')
    }
    triggers {
        cron('H * * * *')
    }
    stages {
        stage('Hello') {
            steps {
                echo "Hello World"
            }
        }
    }
}