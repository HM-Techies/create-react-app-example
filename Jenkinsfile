pipeline {
    agent any

    stages {
        stage('Hello') {
          agent{
            docker{
              image 'node:16-alpine'
            }
            steps {
                sh'''
                npm ci
                npm build
                '''
            }
        }
    }
}
