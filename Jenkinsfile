pipeline {
    agent any

    stages {
        stage('Build'){
            agent{
                docker{
                    image 'node:22.14.0-alpine3.21'
                    reuseNode true
                }
            }
            steps {
                sh '''
                    ls -la
                '''
            }
        }
        // stage('Test'){
        //     agent{
        //         docker{
        //             image 'node:22.14.0-alpine3.21'
        //             reuseNode true
        //         }
        //     }
        //     steps {
        //         sh '''
        //             test -f build/index.html
        //             npm test
        //         '''
        //     }
        // }
    }
}