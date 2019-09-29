pipeline{

 agent any
 
   stages
   {

     stage "scm checkout"{
     git 'https://github.com/ankeetthakkar/maven-project.git'
     }

   }
   {
    
	 stage {'testing test'}{
	 
	     steps{
         withMaven(maven: 'Local Maven') 
		 {
                   sh 'mvn test'
         }
          }

   }
         }
          }
