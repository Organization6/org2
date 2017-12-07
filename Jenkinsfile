#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: https://github.com/Organization6/org2/edit/master/Jenkinsfile,
    pipelineTriggers([githubPush()])])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
