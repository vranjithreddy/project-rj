import jenkins.model.Jenkins
import hudson.model.*
import groovy.json.JsonOutput
import groovy.json.JsonSlurper
import groovy.json.JsonSlurperClassic
import java.text.SimpleDateFormat
  
def version="develop"

def gitCredentials = 'github-cred'  


pipeline {
    agent any {}

    stages {
        stage('get-started') {
            steps {
                script {
                  echo 'get started'
            }
        }
      }
        stage('perform-build') {
                steps {   
                        sh 'pwd'
                        sh 'ls -al'
                }
           }
    }

}
