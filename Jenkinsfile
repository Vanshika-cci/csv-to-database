pipeline {

   agent any
   
   stages {
      stage('Build') {
         steps {
               bat 'mvn -B -U -e -V clean -DskipTests package'
         }
      }
      stage('Test') {
            steps {
                bat 'mvn clean test'
            }
        }
      stage('Deployment') {
         steps {
               bat 'mvn -U -V -e -B -DskipTests deploy -DmuleDeploy -Denvironment=DEV -Dmule.env=dev -Danypoint.username=Vanshika-21 -Danypoint.password=Vans@20021121'
         }
      }
   }
}
