pipeline{
    agent any
    stages{
        stage('git'){
            steps{
                git 'https://github.com/kliakos/sparkjava-war-example.git'
            }
        }
      
      stage('mavenpackage'){
        steps{
           echo 'mvn package'
	   }
	}   
    }
}
