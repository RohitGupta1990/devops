pipeline {
    agent any
    
    stages {
    
    stage ('Checkout') {
    steps {
       git 'https://github.com/devplusopsautomation/devops.git'
    }
    }
    
    stage ('Compile') {
    steps {
       
       sh 'mvn compile'
    }
    }
    
    stage ('Testing') {
    steps {
       sh 'mvn test'
    }
    }
    
    stage ('Package') {
    steps {
       sh 'mvn package'
    }
    }
    
    stage ('Deploy') {
    steps {
       echo 'This is Deploy Stage'
    }
    }
    
    stage ('Notification') {
    steps {
       echo 'This is Notify Stage'
    }
    }
      
    }
