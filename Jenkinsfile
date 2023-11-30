pipeline {
  agent any

  stages {
      stage('Build Artifact') {
            steps {
              sh "mvn clean validate compile package install -DskipTests=true"
              archive 'target/*.jar' //so that they can be downloaded later
            }
        }   
    }
}
