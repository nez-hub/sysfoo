pipeline{

	agent any
	tools{
		maven 'Maven 3.8.2'
	}
	
	stages(

	 stage('build'){
	  steps{
	    sh 'mvn compile'
	  }
	}

        stage('test'){
          steps{
            sh 'mvn clean test'
          }
        }

         stage('package'){
          steps{
            sh 'package -DskipTests'
          }
	 }
        }
}

