pipeline{
    agent any 
    tools {
        maven 'maven3.9.6'
    }
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
}