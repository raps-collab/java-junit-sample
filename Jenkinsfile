node {
   
   stage('Checkout'){
      checkout scm;
   }
   
   stage('Build') {
       
   }

   stage('Test') {
       junit '**/reports/junit/*.xml'
   }

   stage('Deploy') {
       snDevOpsChange();
   }
   
}
