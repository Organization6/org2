#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
     projectUrlStr: 'https://github.com/Organization6/org2.git'],
pipelineTriggers([
        upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/Organization6/org.git'
    )
    ])
    ])
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
