node{
   stage('SCM Checkout'){
     git 'https://github.com/mayukh1/projecturban/blob/master/projecturban'
   }
   stage('Compile-Package'){
      // Get maven home path
      def mvnHome =  tool (name: 'maven_3.5.0', type: 'maven')   
      sh "${mvnHome}/bin/mvn package"
   }
 }