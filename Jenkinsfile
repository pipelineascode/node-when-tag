node{
	stage("Build"){
	/*
		bat 'env > env.txt'
		readFile('env.txt').split("\r?\n").each {
			println it
		}
	*/	
		echo(env.getEnvironment().collect({environmentVariable ->  "${environmentVariable.key} = ${environmentVariable.value}"}).join("\n"))
    echo(System.getenv().collect({environmentVariable ->  "${environmentVariable.key} = ${environmentVariable.value}"}).join("\n"))
		
		
		println "-----"
		println "${env.TAG_NAME}" 
		println "${env.BRANCH_NAME}"
		println "${env.BUILD_TAG}"
		println "${env.CHANGE_ID}"
		println "${env.CHANGE_URL}"
		println "${env.CHANGE_TITLE}"
		println "${env.CHANGE_AUTHOR}"
		println "${env.CHANGE_AUTHOR_DISPLAY_NAME}"
		println "${env.CHANGE_AUTHOR_EMAIL}"
		println "${env.CHANGE_TARGET}"
		println "${env.BUILD_NUMBER}"
		println "${env.BUILD_ID}"
		println "${env.BUILD_DISPLAY_NAME}"
	}
}