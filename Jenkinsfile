pipeline {

  agent any

  stages {

    stage("scm checkout") {
  
       steps {

              git 'https://github.com/rajeev214/maven-simple.git'

       }    
    }
    
    stage("Build") {
    
       steps {
        
         def mvnHm = tool name: 'mvn3', type: 'maven'  
	 sh "'${mvnhm}/bin/mvn' clean package"
       }
    }

  }
}
