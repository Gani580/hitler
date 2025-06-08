pipeline { 
    agent any 
    tools { 
        maven 'Mpipeline { 
    agent any 
    tools { 
        maven 'MVN_HOME' // Ensure name matches configured Maven installation 
    } 
    stages { 
        stage('Checkout') {  
            steps { 
                git branch: 'master', url: 'https://github.com/Gani580/hitler.git'  
            } 
        } 
        stage('Build') {  
            steps { 
                bat 'mvn clean package'  
            } 
        } 
        stage('Test') {  
            steps { 
                bat 'mvn test'  
            } 
        } 
        stage('Run Application') {  
            steps { 
                bat 'java -jar target/hit3-0.0.1-SNAPSHOT.jar'  
            } 
        } 
    } 
}

