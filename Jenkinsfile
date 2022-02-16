pipeline{
    agent any
    tools {
  jdk 'Myjava'
  maven 'mymaven'
    }
    stages{
        stage('git'){
            steps{
                git 'https://github.com/kliakos/sparkjava-war-example.git'
            }
        }
      
      stage('mavenpackage'){
        steps{
           sh 'mvn clean package'
	   }
	}   
    }
}
