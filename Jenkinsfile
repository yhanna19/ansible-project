pipeline {
   agent any 
   //  tools {
   //    maven 'my_maven'
   //    git 'my_git'
   //    ansible 'my_ansible'
   // }
     stages {
   //      stage('Code Compilation') { 
   //       steps { 
   //          echo 'Checking out git repo' 
   //          git url: 'https://github.com/yhanna19/jenkins-project.git'
   //       } 
   //      }
        stage('Invoke Ansible Playbook'){
           steps {
              ansiblePlaybook(playbook: 'jenkins.yml')
           }
        }
    }
}