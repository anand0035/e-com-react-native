pipeline{
    agent any
    environment {
            //Fastlane Environment Variables

           APP_NAME = "DEMO_APP"
            LC_ALL = "en_US.UTF-8"
            LANG = "en_US.UTF-8"

        }

    stages
    {
//         stage('npm install'){
//             steps{
//                 bat 'npm install'
//             }
//         }
//         stage('testing your code'){
//             steps{
//                 bat 'npm run test'
//             }
//         }
        stage('build android'){
            steps{
                sh "chmod +x gradlew"
                sh "/var/lib/gems/3.0.0/gems/fastlane-2.208.0/bin/fastlane"
                sh "Fastlane android test"
            }
        }
    }
}

