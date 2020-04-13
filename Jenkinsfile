pipeline {
    agent any

    stages {
        stage('Deploy code on all branches except branches which starts with vx.x') {
            steps {
                script {
                    
                    if(!(env.BRANCH_NAME ==~ /^v([0-9]+\.[0-9])/)) {
        buildTag = "${env.BRANCH_NAME}-${env.BUILD_NUMBER}"
        branchNamePlaceholder = "-${env.BRANCH_NAME}"
	    echo "test"
		    }else { echo "tested"}
                }
            }
        }
    }
}
