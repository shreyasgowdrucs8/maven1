pipeline { 
    agent any 
 
    tools { 
        
        maven 'Maven3' 
    } 
 
    stages {
       stage('CHECKOUT') { 
            steps { 
                git 'https://github.com/shreyasgowdrucs8/maven1.git' 
            } 
        } 
 
        stage('Build') { 
            steps { 
                dir('demo'){ 
                bat 'mvn clean install' 
            } 
            } 
        } 
        stage('Test') { 
            steps { 
                dir('demo'){ 
                bat 'mvn test' 
            } 
            } 
        } 
    }    
}
