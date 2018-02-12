pipeline {
    agent any
    stages {
        stage('checkout into project'){
          steps{
            sh 'cd Sample-webapp'
            }
           }
         stage('mvn generate'){
         steps{
         sh 'mvn archetype:generate'
         }
         }
         stage('package'){
         steps{
         sh 'mvn package'
         }
         }
         stage('add file'){
         steps{
         sh 'git add .'
         }
         }
        stage('commit changes'){
         steps{
         sh 'git commit -am "trying from jenkins"'
         }
         }
    stage('push'){
         steps{
         sh 'git push origin master'
         }
         }

stage('message') {
            steps {
                sh 'echo "successfully finished"'
         
                
            }
        }
    }
}
