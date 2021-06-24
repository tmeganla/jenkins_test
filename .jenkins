// Test pipeline
pipeline {
    agent {
        label {
            label "irvapp069.ir.intel.com"
        }
    }
    stages {
        stage('Hello') {
            steps {
                cleanWs()
                echo 'Hello World'
				sh 'printenv'
				sh """
				git clone https://github.com/tmeganla/jenkins_test/
				ls -l 
				"""
				cleanWs()
            }
        }
    }
}
