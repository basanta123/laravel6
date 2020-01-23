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
                    if (env.BRANCH_NAME.contains('dev')) {
                        echo 'This is not master but for sandbox'
                    } else {
                        echo 'things and stuff'
                    }
                }
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