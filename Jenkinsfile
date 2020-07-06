pipeline {
    agent any
    stages {
      steps ('clone-master') {
         when {
         branch 'master'
         }
         stage ('build'){
            steps {
              echo "clone master"
            }
         }


      }
      steps ("clone-qa") {
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
