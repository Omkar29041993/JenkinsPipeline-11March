node {
    stage('Git Checkout'){
	   def branchName = getCurrentBranch()
        echo 'My branch is' + branchName
        
        def getCurrentBranch () {
        return sh (
            script: 'git rev-parse --abbrev-ref HEAD',
            returnStdout: true
        ).trim()
    }
}
