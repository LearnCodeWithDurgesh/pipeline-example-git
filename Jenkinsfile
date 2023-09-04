pipeline{

    agent any 
    stages{

        stage("compile"){
               
               sh 'javac Test.java'

        }

        stage("run"){

            sh "java Test"

        }
    }

}