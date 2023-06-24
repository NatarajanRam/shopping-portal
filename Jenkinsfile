pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'nodejs' 
    }
*/    

    stages{
        stage('Build'){
            steps{
                echo 'this is the build job'
                sh 'npminstall'
                
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
                
            }
        }
        stage('three'){
            steps{
                echo 'this is the Packaage job'
                sh 'npm package'
                
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
