pipeline {

   agent any
   
   stages {
      stage('Build') {
         steps {
               bat 'mvn -B -U -e -V clean -DskipTests package'
         }
      }
<<<<<<< HEAD
=======
      stage('Test') {
            steps {
                bat 'mvn clean test -U'
            }
        }
>>>>>>> e2e6106b6ce577d112d91ab8c3de19808df50d1a
      stage('Deployment') {
         steps {
               bat 'mvn -U -V -e -B -DskipTests deploy -DmuleDeploy -Denvironment=DEV -Dmule.env=dev -Danypoint.username=Vanshika-21 -Danypoint.password=Vans@20021121'
         }
      }
   }
}
