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
                git clone https://github.com/HM-Techies/create-react-app-example.git
                  ls -la > b.txt
                npm install
                npm build
                la -la > a.txt
                '''
            }
        }
    }
}
