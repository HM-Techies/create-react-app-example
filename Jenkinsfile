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
                  ls -la > b.txt
                npm install
                npm build
                la -la > a.txt
                '''
            }
        }
    }
}
