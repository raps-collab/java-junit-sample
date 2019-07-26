node {
   
   stage('Checkout'){
      checkout scm;
   }
   
   stage('Build') {
       
   }

   stage('Test') {
       junit '**/test-results/test/*.xml'
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
