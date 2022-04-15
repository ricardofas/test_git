node("master"){
  stage("checkout"){
    def scmVars = checkout scm
    def commitHash = scmVars.GIT_COMMIT
    println commitHash
  }
}
