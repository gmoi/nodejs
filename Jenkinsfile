#!/usr/bin/env groovy

import jenkins.model.*

node {
  stage('Build') {
    awsCodeBuild projectName: "testcb", region: "us-east-1", sourceControlType: "project", credentialsId: "$JENKINS_CREDENTIAL_ID", credentialsType: "jenkins"
  }
}
