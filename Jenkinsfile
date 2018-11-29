pipeline {

  agent any

  stages {

    stage("scm checkout") {
  
       step {

              git 'https://github.com/rajeev214/maven-simple.git'

       }    
    }
    
    stage("Build") {
    
       step {
        
           def mvnhm
	   mvnhm = tool mvn3
           sh '${mvnhm}/bin/mvn clean package'
       }
    }

  }
}
