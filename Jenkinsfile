pipeline {
    agent any
    stages {

        stage('Deliver for sandbox') {
            when {
                branch 'develop'
            }
            steps {
               echo " Delivering to sandbox";
               script { 
                    if (env.BRANCH_NAME.contains('feature')) {
                        echo 'This is only for feature branch'
                    } 
                }
                echo "Not delivering to feature";
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