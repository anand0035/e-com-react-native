pipeline{
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
        stage('build android'){
            steps{
                 bat 'icacls "android/gradlew" /grant Users:F'
                bat "Fastlane android build"
            }
        }
    }
}


}
