pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'Maven 3.6.3' 
    }
    

    stages{
        stage('build'){
            steps{
                echo 'this is the first job'
                sh 'compile'
            }
        }
        stage('test'){
            steps{
                echo 'this is the second job'
                sh 'clean test'
            }
        }
        stage('three'){
            steps{
                echo 'this is the third job'
                sh 'package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed for shopping-carts...'
        }
        
    }
    
}
