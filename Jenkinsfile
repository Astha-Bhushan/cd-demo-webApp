pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		                sh 'ls -ltr'  //linux ls -lrt command, sorts non-hidden files and directories by date from old to new. //
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install helm-dep petclinic-chart  --set image.repository=https://hub.docker.com/repository/docker/asthabhushan/cicd-demo --set image.tag=1'
              			
            }           
        }
    }
}
