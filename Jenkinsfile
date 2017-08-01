pipeline {
 agent any
  stages {
    stage ('build') {
      steps {
        sh 'javac -d . src/.java'
        sh 'echo Main-class: Rectangular > MANIFEST.MF'
        sh 'jar -cvmf MANIFEST.MF rectangular.jar .class'
       }
     }
    }
   }
