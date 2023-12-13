pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('build-app'){
            steps{
                echo 'this is the build job'
                sh 'npm install'
            }
        }
        stage('test-app'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
            }
        }
        stage('package-app'){
            steps{
                echo 'this is the Package job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
