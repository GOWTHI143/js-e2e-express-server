pipeline{
    agent {label 'Nodejs'}
    stages{
        stage ('scm'){
            steps{
                git url:"https://github.com/GOWTHI143/js-e2e-express-server.git",
                branch:"main"
            }
         }
        stage ('build') {
            steps{
                sh """sudo apt install npm -y
                    sudo npm install"""
            }
        }
        stage ('start'){
            steps{
                sh "sudo npm start"
            }
        }
    }
}