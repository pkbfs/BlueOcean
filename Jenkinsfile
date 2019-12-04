pipeline {
  agent any
  stages {
    stage('StageOne') {
      steps {
        sh '#'
      }
    }

    stage('StageTwo') {
      parallel {
        stage('StageTwo') {
          steps {
            echo 'StageTwo'
          }
        }

        stage('StageTwoB') {
          steps {
            echo 'StageTwoB'
          }
        }

        stage('StageTwoC') {
          steps {
            echo 'StageTwoC'
          }
        }

      }
    }

    stage('StageThree') {
      steps {
        echo 'StageThree'
      }
    }

    stage('StageFour') {
      parallel {
        stage('StageFour') {
          steps {
            echo 'StageFour'
          }
        }

        stage('StageFourA') {
          steps {
            echo 'StageFourA'
          }
        }

        stage('StageFourB') {
          steps {
            echo 'StageFourB'
          }
        }

      }
    }

    stage('StageFive') {
      steps {
        echo 'StageFive'
      }
    }

    stage('FinalStage') {
      steps {
        echo 'FinalStage'
      }
    }

  }
}