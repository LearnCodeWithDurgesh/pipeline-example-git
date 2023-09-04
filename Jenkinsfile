pipeline{

    agent any 
    stages{
        

        stage("compile"){
               
            steps{
                   sh 'javac Test.java'
            }

        }

        stage("run"){

           steps{
             sh "java Test"
           }

        }
    }

    post{

        always {

            sh 'echo "always"'
        }

        success{
            sh 'echo "success"'
        }

        failure{
            sh 'echo "failure"'
        }

    }

}