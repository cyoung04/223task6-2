pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                echo "Build the code using a build automation tool to compile and package your code..."
            }
        }
        stage("Unit and Integration Tests"){
            steps{
                echo "Run unit tests to ensure the code functions as expected and run integration tests to ensure the different components of the application work together as expected..."
            }
            post{
                success{
                   mail to: "cyoung1902@gmail.com",
                   subject: "Tests Status Email",
                   body: "Unit and Integration tests were successful" 
                }
            }
        }
        stage("Code Analysis"){
            steps{
                echo "Integrate a code analysis tool to analyse the code and ensure it meets industry standards..."
            }
        }
        stage("Security Scan"){
            steps{
                echo "Perform a security scan on the code using a tool to identify any vulnerabilities..."
            }
            post{
                success{
                   mail to: "cyoung1902@gmail.com",
                   subject: "Security Scan Status Email",
                   body: "Security scan was successful" 
                }
            }
        }
        stage("Integration Tests on Staging"){
            steps{
                echo "Run integration tests on the staging environment to ensure the application functions as expected in a production-like environment..."
            }
            post{
                success{
                   mail to: "cyoung1902@gmail.com",
                   subject: "Integration Tests on Staging Status Email",
                   body: "Integration tests on staging were successful" 
                }
            }
        }
        stage("Deploy to Production"){
            steps{
                echo "Deploy the application to a production server..."
            }
        }
    }
}
