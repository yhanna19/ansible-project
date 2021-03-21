pipeline {
    agent any
    tools {
        maven ​'my_maven'
        git ​'my_git' 
    }
    stages {
        stage(​'Code Compilation'​) {
            steps {
​               echo​ ​'Building Code'
               sh ​'mvn compile' 
            }
        }
    }
}