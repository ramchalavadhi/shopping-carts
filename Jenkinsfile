pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'maven' 
    }
    

    stages{
        stage('compile-app'){
            steps{
                echo 'this is the compile job'
                sh 'mvn compile'
            }
        }
        stage('test-app'){
            steps{
                echo 'this is the test job'
                sh 'mvn test'
            }
        }
        stage('package-app'){
            steps{
                echo 'this is the package job'
                sh 'mvn package'
            }
        }
    }
    
    post{
        always{
            echo 'Hey, this is my second pipeline as code... SUCCESS'
        }
        
    }
    
}
