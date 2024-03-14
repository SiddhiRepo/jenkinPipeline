pipeline{
    agent any
    stages{
        stage("compile"){
            steps{bat 'javac Test.java'}

        }
        stage("run"){
         steps{bat "java Test"}   
        }
    }
    post{
        success {
            sh 'echo "Success"'
        }
        always {
            sh 'echo "Always"'
        }
        
    }
}
