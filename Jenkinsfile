
def gv
pipeline {
  agent any
  parameters {
      //choice(name: 'VERSION', choices: ['1.1', '1.2'], description: '')
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
        stage ('build')
          steps {
              script{
                  gv.buildApp()
              }
=======
    stages {
        stage('Build') { 
            steps {
                echo "Build from Git.."
            }
>>>>>>> 8ff9ce449590e7c2767c04adb1711ef530444f8f
        }
    }
}
