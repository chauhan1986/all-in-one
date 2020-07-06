pipeline {
    agent any
    stages {
      stage ('clone-master') {
         when {
         branch 'master'
         }
         stage ('build'){
            steps {
              echo "clone master"
            }
         }


      }
      stage ("clone-qa") {
         when {
         branch 'qa'
         }
         stage ("build"){
            steps {
              echo "clone qa"
            }
         }


      }
      stage ("clone-dev") {
         when {
         branch 'dev'
         }
      }
      stage ("build"){
            steps {
              echo "clone dev"
            }
         }

    }
}
