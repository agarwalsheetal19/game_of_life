pipeline {
 agent any
 stages {
 stage('build') {
 steps {
 sh 'mvn clean package'
 sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
 }
 }
post {
 success {
 archiveArtifacts artifacts: 'gameoflife-web/*.jar', fingerprint:
true
 }
 }
 }
}
