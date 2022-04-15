node("master"){
  stage("checkout"){
    def scmVars = checkout scm
    def commitHash = scmVars.GIT_COMMIT
    def commitshortHash = sh(script: "printf \$(git rev-parse --short ${commitHash})",returnStdout: true)
    println "Commit hash is:"+commitHash
    println "Commit short hash is:"+commitshortHash
  }
}
