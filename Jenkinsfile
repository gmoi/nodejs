#!/usr/bin/env groovy

import jenkins.model.*

node {
  stage('Build') {
    awsCodeBuild projectName: "$CODEBUILD_PROJECT_NAME", region: "$REGION", sourceControlType: "project", credentialsId: "$JENKINS_CREDENTIAL_ID", credentialsType: "jenkins"
  }
}
