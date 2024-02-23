pipeline{
    agent any 
    stages {
        stage('Git Checkout'){
            steps{
                script{
                    git branch: 'main', url: 'https://github.com/ericsewoe/demo-counter-app.git'
                }
            }
        }

        stage ("UNIT Test"){
            steps {
                sh 'mvn test'
            }
    }   
}