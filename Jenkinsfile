pipeline{
    agent any
    stages{
       
            stage("compile")
            {
                steps
                {
                    bat 'javac Test.java'
                }
            }

            stage("run")
            {
                steps
                {
                    bat "java Test"
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
