pipeline {
   agent any
   stages{
   stage('Build') {
   steps {
   echo 'Running Build'
   }
   }
   stage('Test ') {
            steps {
               input 'Does Build environment look ok?'
            }
   }
      stage('Production ') {
            steps {
               input 'Does Test environment look ok?'
            }
   }
   }
}
