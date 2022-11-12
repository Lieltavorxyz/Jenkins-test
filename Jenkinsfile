// pipeline{
//     agent any
    
//     stage('Build'){
//         steps {
//             sh ' echo build ..... '
//         }
//     }
//     stage('test'){
//         steps {
//             echo 'testing ......'
//         }
//     }
//     stage('Deploy'){
//         steps {
//             echo 'Deployinggg......... '
//         }
//     }
//     stage('Party'){
//         steps {
//             echo 'Partyinggg.......... Moon walk MJ'
//         }
//     }
// }

pipeline{
    agent any

    environment {
        NAME = 'Liel Tavor'
        cloneRepo = ''
        DHCU = '' // Docker Hub Credentials Password
        DHCP = '' // Docker Hub Credentials Password
    }
    stages {
        stage ('Fetching......') {
            steps {

                sh 'echo your name is $(NAME) '
                timeout(time: 10, unit: 'SECONDS') {
                sh '''
                    sleep 5
                    echo "Hello"
                    ls -lah
                    ping -c 3 www.google.com
                '''
            }
        }
    }
            stage ('Build......') {
                
            steps {
            retry (3)
                sh '''
                sleep 3
                echo "Finished"
                '''
                }
            }
        }
}