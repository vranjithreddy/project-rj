import jenkins.model.Jenkins
import hudson.model.*
import groovy.json.JsonOutput
import groovy.json.JsonSlurper
import groovy.json.JsonSlurperClassic
import java.text.SimpleDateFormat
  
def version="develop"

def gitCredentials = 'github-cred'  


pipeline {
    agent any //{ dockerfile true } 

 // tools {nodejs "nodejs"}

    stages {
        stage('get-started') {
            steps {
                script {
                  echo 'get started'
            }
        }
      }
        stage('npm-install') {
                steps {  
                  withDockerContainer('node:latest') {
                     sh "npm install"
                   }
                }
           }
        stage('npm run lint') {
                steps {   
                     sh "npm run lint"
                }
           }
        stage('npm run test') {
                steps {   
                     sh "npm run test"
                }
           }
        stage('npm run test only changed') {
                steps {   
                     sh "npm run test:onlychanged"
                }
           }
    }

}
