pipeline{

    agent any 
    environment{

            VERSION_NAME="1.34"


    }
    stages{
        

        stage("compile"){
               
            steps{
                   sh 'javac Test.java '
                   sh 'echo "${VERSION_NAME}"'
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