pipeline{

 agent any
 
   stages
   {

     stage "scm checkout"{
     git 'https://github.com/ankeetthakkar/maven-project.git'
     }

   }
   {
    
	 stage ('testing stage'){
	 
	     steps{
              withMaven(maven: 'Local Maven') 
		     {
               sh 'mvn test'
             }
              }

   }
   
   {
     stage ('Testing package'){
	    
		steps{
		   withMaven(maven: 'Local Maven')
		   {
			 sh 'mvn package'
		   }
		     {
       }
          }
