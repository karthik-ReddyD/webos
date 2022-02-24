pipeline{
    agent any
    tools {
  jdk 'Myjava'
  maven 'mymaven'
    }
	environment {
  mygiturl = "https://github.com/kliakos/sparkjava-war-example.git"
}
    stages{
        stage('git'){
            steps{
                git '$mygiturl'
            }
        }
      
      stage('mavenpackage'){
        steps{
           sh 'mvn clean package'
	   }
      }
	      stage('deploy'){
		      steps{
			 sh 'mvn clean deploy'     
		      }
	      }   
    }
}
