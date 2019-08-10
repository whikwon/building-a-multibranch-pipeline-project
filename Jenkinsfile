pipeline {
    agent {
		docker {
			image 'nvidia/cuda:9.0-base'
			args '--runtime nvidia'
		}
	}
    stages {
        stage('Build') {
            steps {
				sh 'nvidia-smi'
                sh 'echo "Hello world!"'
            }
        }
    }
}
