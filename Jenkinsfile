pipeline{
    agent any
    stages{
        stage('git'){
            steps{
                echo 'git checkout'
            }
        }
      
      stage('mavenpackage'){
        steps{
           echo 'mvn package'
	   }
	}   
    }
}
