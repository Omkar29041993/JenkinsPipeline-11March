node {
   sh 'git name-rev --name-only HEAD > GIT_BRANCH'
   sh 'cat GIT_BRANCH'
	// sh 'cat GIT_BRANCH'
	// git_branch = readFile('GIT_BRANCH').trim()
	// env.GIT_BRANCH = git_branch
	// echo "GIT_BRANCH=$GIT_BRANCH"
	sh 'echo Branch Name: $GIT_BRANCH'
	// sh 'git rev-parse HEAD > commit'
	// def commit = readFile('commit').trim()
	// echo "commit=$commit"
	env.GIT_BRANCH_PATH=sh(returnStdout: true, script: "git name-rev --name-only HEAD").trim()
    env.GIT_BRANCH_NAME=GIT_BRANCH_PATH.split('remotes/origin/')[1]
    sh 'echo Branch Path: $GIT_BRANCH_PATH'
    sh 'echo Branch Name: $GIT_BRANCH'
}
