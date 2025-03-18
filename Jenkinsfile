pipeline {
     agent any
     stages {
       
         stage('Build') {
             steps {
                 script {
                     build 'PES1UG22CS702'
                     sh 'g++ -o yu sy 6vr i a new_cpp_file. cpp This is an intentional edit made to make this fail.'
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
                  Making another random intentional edit to fail the jenkinsfile
             }
         }
     }
 
     post {
         failure {
             echo 'You made an error. Pipeline has failed'
         }
     }
 }
