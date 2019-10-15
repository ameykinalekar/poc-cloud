
node {
   stage('SCM Checkout'){ 
	url: 'https://github.com/ameykinalekar/poc-cloud'   
   }
   stage('Mvn Package'){
      def mvn = tool name: '', type: 'maven' + '/bin/mvn'
	   // Build using maven
	sh "${mvn} clean package deploy"
   }
