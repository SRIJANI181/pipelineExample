pipeline{
    agent any
    stages{
       
            stage("compile")
            {
                steps
                {
                    sh 'javac Test.java'
                }
            }

            stage("run")
            {
                steps
                {
                    sh "java Test"
                }
            }
        }

        post{

            always
            {
                echo "always"
            }

            success
            {
                echo "build success"
            }
            failure
            {
                echo "failure"
            }
        }
    }
