node("master"){
  stage("checkout"){
    def scmVars = checkout scm
    def commitHash = scmVars.GIT_COMMIT
    def commitshorthash = sh(script: "printf \$(git rev-parse --short ${commitHash})",returnStdout: true)
    println commitHash
    println commitshortHash
  }
}
