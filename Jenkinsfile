pipeline {
    agent any
    stages {
        stage('Start') {
            steps {
                echo "world"
            }
        }
        stage('upload') {
	    	when {
    		    expression {
        	    env.TAG_NAME != null
                    }
                }
                steps {
                    echo "hello,${env.TAG_NAME}"
		}
	}
    }
}
