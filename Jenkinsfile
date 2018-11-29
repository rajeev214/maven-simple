pipeline {

  agent any

    def mvnhm
  stages {

    stage("scm checkout") {
  
       steps {

              git 'https://github.com/rajeev214/maven-simple.git'

       }    
    }
    
    stage("Build") {
    
       steps {
        
	   mvnhm = tool 'mvn3'
           sh "'${mvnhm}/bin/mvn' clean package"
       }
    }

  }
}
