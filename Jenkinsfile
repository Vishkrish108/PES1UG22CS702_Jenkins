pipeline {
     agent any
     stages {
       
         stage('Build') {
             steps {
                 script {
                     build 'PES1UG22CS702'
                     sh 'g++ -o a PES1UG22CS702.cpp'
                 }
             }
         }
 
         stage('Test') {
             steps {
                 script {
                     sh './a'
                 }
             }
         }
 
         stage('Deploy') {
             steps {
                 echo 'This pipeline works!!!'
             }
         }
     }
 
     post {
         failure {
             echo 'You made an error. Pipeline has failed'
         }
     }
 }
