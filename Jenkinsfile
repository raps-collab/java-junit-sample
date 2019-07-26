node {
   
   stage('Checkout'){
      checkout scm;
   }
   
   stage('Build') {
       
   }

   stage('Test') {
       sh 'mvn test';
   }

   stage('Deploy') {
       snDevOpsChange();
   }

   post {
      always {
        junit '**/reports/junit/*.xml'
      }
   } 
   
}
