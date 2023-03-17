import jenkins.model.Jenkins
import hudson.model.*
import groovy.json.JsonOutput
import groovy.json.JsonSlurper
import groovy.json.JsonSlurperClassic
import java.text.SimpleDateFormat
  
def version="develop"

def gitCredentials = 'github-cred'  


pipeline {
    agent { dockerfile true } 

    stages {
        stage('get-started') {
            steps {
                script {
                  echo 'get started'
            }
        }
      }
        stage('docker-build') {
                steps {   
                     sh "docker build -t project-rj ."
                }
           }
    }

}
