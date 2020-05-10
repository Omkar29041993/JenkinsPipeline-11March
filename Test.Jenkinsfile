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
}
