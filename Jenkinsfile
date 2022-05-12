pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
              // bat "rmdir  /s /q TicketBookingServiceJunitTesting"
                bat "git clone https://github.com/kishancs2020/TicketBookingServiceJunitTesting.git"
              //  bat "mvn clean -f TicketBookingServiceJunitTesting"
            }
        }
        stage('install') {
            steps {
              //  bat "mvn install -f TicketBookingServiceJunitTesting"
                echo "Install step" 
            }
        }
        stage('test') {
            steps {
                echo "test step"
              //  bat "mvn test -f TicketBookingServiceJunitTesting"
            }
        }
        stage('package') {
            steps {
                echo "Package"
              //  bat "mvn package -f TicketBookingServiceJunitTesting"
            }
        }
    }
}
