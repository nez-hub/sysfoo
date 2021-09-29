pipeline{

	agent any
	tools{
		maven 'Maven 3.8.2'
	}
	
	stages(

	 stages('build'){
	  steps{
	    sh 'mvn compile'
	  }
	}
	stages(

         stages('test'){
          steps{
            sh 'mvn clean test'
          }
        }
	stages(

         stages('package'){
          steps{
            sh 'package -DskipTests'
          }
	 }
}

