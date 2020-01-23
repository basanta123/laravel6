pipeline {
    agent any
    stages {

        stage('Deliver for sandbox') {
            when {
                branch 'develop'
            }
            steps {
               echo " Delivering to sandbox";
            }
        }

        stage('Deliver for production') {
            when {
                branch 'master'
            }
            steps {
               echo " Delivering to production";

            }
        }
        
    }
}