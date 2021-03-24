pipeline {
	
  agent any
  stages {
        stage('Build Application') {
            steps {
                  bat 'mvn clean install'
                  }
         }
          stage('Deploy Application into cloudhub') {
                steps {
                      bat "mvn clean package deploy -Dmuledeploy"
                }
            }
        }
    }
}
