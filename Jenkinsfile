pipeline {
   agent any
   stages{
   stage('Build') {
   steps {
   echo 'Running Build'
   }
   }
   stage('Test ') {
            when {
                branch 'master'
            }
            steps {
               input 'Does Build environment look ok?'
            }
   }
      stage('Production ') {
            when {
                branch 'master'
            }
            steps {
               input 'Does Test environment look ok?'
            }
   }
   }
}
