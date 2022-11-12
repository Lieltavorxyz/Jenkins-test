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
    stages {
        stage ('Fetching......') {
            steps {
                timeout(time: 3, unit: 'SECONDS') {

                sh '''
                    sleep 5
                    echo "Hello"
                    ls -lah
                    ping www.google.com
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