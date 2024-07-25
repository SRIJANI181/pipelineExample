pipeline{
    agent any
    stages{
       
            stage("compile")
            {
                steps
                {
                    echo 'javac Test.java'
                }
            }

            stage("run")
            {
                steps
                {
                    echo "java Test"
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
