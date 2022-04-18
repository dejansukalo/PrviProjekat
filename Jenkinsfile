
def gv
pipeline {
  agent any
  parameters {
      choice(name: 'VERSION', choices: ['1.1', '1.2'], description: '')
      booleanParam(name: 'executeTest', defaultValue: true, description: '')
  }
  stages {
      stage('init') { 
         steps {
             script{
                 gv = load "script.groovy"
             }
           }
        }
        stage ('build') {
          steps {
              script{
                  gv.buildApp()
              }
            }
        }
    }
}
