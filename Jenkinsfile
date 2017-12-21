pipeline {
   agent any 	
   staegs {
       stage ('Sonar'){
          steps{
		echo'This is sonar stage'
	  }

        }

	stage ('Build') {
	   steps{
	   	echo 'Buling code here'
           }
	}

	stage ('Deplo') {
	   steps {
	   echo 'Project Deploying here'
           }

	}
    }

}
