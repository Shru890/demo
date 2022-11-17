pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
           echo "build success"    
      }
    }

    stage('Test') {
      steps {
          echo "mvn test"
      }
    }

     stage('Deploy Development') {
      steps {
            bat "mvn clean package deploy -DmuleDeploy -Dusername=shru_0506 -Dpassword=Puk@1974 -Dappname=assignment-19-udaan-nair -Dworker=1 -Dworkertype=MICRO -Denv=Sandbox"
            echo "deploy success"           
      }
    }
}
}
