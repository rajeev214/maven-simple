pipeline {

  agent any

  stages {

    stage("scm checkout") {
  
       steps {

              git 'https://github.com/rajeev214/maven-simple.git'

       }    
    }
    
    def mvnhm
    stage("Build") {
    
       steps {
        
	   mvnhm = tool 'mvn3'
           sh "'${mvnhm}/bin/mvn' clean package"
       }
    }

  }
}
