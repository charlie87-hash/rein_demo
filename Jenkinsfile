def recipients = [slack: '#nt-restarts']
def gitRepo = "git@gh.**********.com:cpt/rein.git"
def credentialsId = "****************" // for svc-ekko
def workDir = "/home/jenkins/go/src/go.*************.com/cpt/rein"
def buildAgent = "pipe-default-go-slave"
def timeout = 10 // minutes

pipeline
{
    agent any

    stages{
        stage('Get latest rein release'){
            steps
                {
                //Get the latest release for_linux
                echo 'Getting latest release for linux'
            }
        }
        stage('Run rein fetch'){
            steps
                {
                echo 'Running rein fetch'
                //Authenticate with AWS credentials and assume AWS role using ekko_pass service account
                echo 'Authenticate with AWS credentials and assume AWS role using ekko_pass service account'
                //pull eC2 instances that are due restart inthe AWS events section
                echo 'Getting eC2 instances that are due restart inthe AWS events section '
                //create jira ticket
                echo 'Creating Jira Tickets'
                //notify slack (can be post action)
                echo 'Notifying slack that job was successful'
                
            }
        }
        stage('rein bounce'){
                steps
                    {
                    echo 'running rein bounce'
                    //open cli using groovy ***.execute()
                    echo 'open cli using groovy ***.execute()'
                    // assume AWS role using ekko_pass service account (MFA can be set in Jenkins credentials as well)
                    echo 'assume AWS role using ekko_pass service account'
                    //Use ekko_pass to get jira ticket from the epic
                    echo 'ekko_pass to get Jira ticket from epic repo'
                    //Create change ticket
                    echo 'Create change ticket'
                    //Notify NOC
                    echo 'notifying #ask_live_noc and #nt_clops'
                    //Use ekko_pass to get the FDQN and instance tags
                    echo'Getting instance ID and service tags'
                    //use the ekko_pass service account to ssh into the defined instance
                    echo ' ssh into defined instance'
                    //with matched tags and the considerations stop the services e.g tomcat before stopping the instance
                    echo 'Stopping services'
                    //(you may use interactive session with jenkins)
                    echo 'Do you want to continue? yes, hit enter, no to interupt session'
                    //stop/ start the instance(wait time)
                    echo 'stop the instance'
                    echo 'starting the instance'
                    //start the service that was stopped
                    echo 'Starting services'
                    //close change ticket
                    echo 'Closing change ticket'
                    //notify the NOC
                    echo 'Change Ticket was executed successfully'
                }
        }
    }
}
