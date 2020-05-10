node {
    stage('Git Checkout'){
	echo "Git Checkout"
        // FULL_PATH_BRANCH = "${sh(script:'git name-rev --name-only HEAD', returnStdout: true)}"
        // GIT_BRANCH = FULL_PATH_BRANCH.substring(FULL_PATH_BRANCH.lastIndexOf('/') + 1, FULL_PATH_BRANCH.length())
        // echo "My branch is: ${env.BRANCH_NAME}"
        // echo 'Pulling...' + env.BRANCH_NAME
        // checkout scm
        def BRANCH = sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()
    	echo ${BRANCH}
   }
}
