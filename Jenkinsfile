pipeline {

  agent any

  tools {
        maven 'mvn3' 
    }
  stages {

    stage("scm checkout") {
  
       steps {

              git 'https://github.com/rajeev214/maven-simple.git'

       }    
    }
    
    stage("Build") {
    
       steps {
        
	 sh "mvn clean package"
       }
    }

  }
}
