def builderImage
def productionImage
def ACCOUNT_REGISTRY_PREFIX
def GIT_COMMIT_HASH

pipeline {
  aggent any
  stages('Checkout Source Code and Logging Into Registry') {
    steps {
      echo 'Logging Into the Private Registry'
      script {
        GIT_COMMIT_HASH = sh (script: "git log -n 1 --pretty=format:'%H'", returnStdout: true)
        ACCOUNT_REGISTRY_PREFIX = "git@github.com:giemar11"
      }
    }  
  }  
}
