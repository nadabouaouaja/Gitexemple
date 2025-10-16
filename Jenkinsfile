pipeline {
  agent any
  tools { jdk 'JDK17' }
  stages {
    stage('Checkout code') {
      steps { git branch: 'master', url: 'https://github.com/nadabouaouaja/Gitexemple.git' }
    }
    stage('Compile code') {
      steps { sh 'javac HelloWorld.java' }
    }
    stage('Execute code') {
      steps { sh 'java HelloWorld ' }
    }
  }
}

