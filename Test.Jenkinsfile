node {
	sh 'echo Branch Name: $GIT_BRANCH'
	env.GIT_BRANCH_PATH=sh(returnStdout: true, script: "git name-rev --name-only HEAD").trim()
    env.GIT_BRANCH_NAME=GIT_BRANCH_PATH.split('remotes/origin/')[1]
    sh 'echo Branch Path: $GIT_BRANCH_PATH'
    sh 'echo Branch Name: $GIT_BRANCH_NAME'
}
