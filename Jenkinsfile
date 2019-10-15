
node {
   def mvn = tool name: '', type: 'maven' + '/bin/mvn'
   stage('SCM Checkout'){ 
	url: 'https://github.com/ameykinalekar/poc-cloud/'   
   }
   stage('Mvn Package'){
	   // Build using maven
	sh "${mvn} clean package deploy"
   }
   
