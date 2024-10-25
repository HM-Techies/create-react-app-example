pipeline {
    agent any

    stages {
        stage('Hello') {
          agent{
            docker{
              image 'node:16-alpine'
            }
            }
            steps {
                sh'''
                ls -la
                cd create-react-app-example
                npm i
                npm run build
                '''
            }
        }
    }
}
