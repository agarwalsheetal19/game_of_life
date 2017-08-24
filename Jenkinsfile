pipeline {
 agent any
 stages {
 stage('build') {
 steps {
 sh 'mvn clean package'
 }
 }
 }
post {
 success {
 archiveArtifacts artifacts: 'gameoflife-web/target/gameoflife.war', fingerprint:
true
 }
 }

}
