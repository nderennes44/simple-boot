pipeline {
    agent any 
    
    tools{
        maven 'M3'
        
    }
    
    stages {
        stage ('Checkout'){
            steps {
                git url:'https://github.com/nderennes44/simple-boot.git'
            }
            
        }
        
        stage ('Compile'){
            steps{
                sh 'mvn clean compile'
        }
        }
        
        stage ('test'){
            steps{
                sh 'mvn test'
            }
        }
            
            stage ('Package'){
                steps {
                    sh 'mvn package'
                
                }
    }
}
        
    