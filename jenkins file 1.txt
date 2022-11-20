pipeline {
 agent  { label "ECSagent"}
  stages {
     stage ('source') {
             steps {
                git 'https://github.com/karthicak/my-project'
             }
        }
     stage('Running Build') {
       steps {
         echo "Hello World !@"
       }
     }
  }
}