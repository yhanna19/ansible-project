pipeline {
   agent any 
    tools {
      maven 'my_maven'
      git 'my_git'
   }
    stages {
        stage('Code Compilation') { 
         steps { 
            echo 'Checking out git repo' 
            git url: 'https://github.com/yhanna19/jenkins-project.git'         
            sh 'mvn compile' 
         } 
        }
        stage('Ansible Init'){
           steps {
              script {
                 def tfHome = tool name: 'Ansible'
                 env.PATH = "${tfHome}:${env.PATH}"
                 sh 'ansible --version'
              } 
           }
        }
    }
}