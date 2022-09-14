pipeline {
    agent {
        node {
            label 'built-in'
            customWorkspace '/project/docker-deploy'
        }
    }
    stages {
        stage('clone') {
            steps {
				sh "rm -rf *"
                sh "git clone -b master https://github.com/vinay-aws/Assignment-1.git q1"
			}
        }
		stage('deploy') {
            steps {
				sh 'cp q1/index.html /mnt/VNY'
				}
			}
		}
	}
}
