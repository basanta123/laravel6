pipeline {
    agent any
    stages {

        when {
            branch 'develop'
       

            stage('Deliver for sandbox') {
            
                steps {
                echo " Delivering to sandbox";
                }
            }
        }
        when {
                branch 'master'
            
                stage('Deliver for production') {
                    
                    steps {
                    echo " Delivering to production";

                    }
                }
        }
        
    }
}