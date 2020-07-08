pipeline {
   agent any 
          stages  {
                 stage('COMPILE') {
                                                   steps  {
                                                                   git 'https://github.com/kushalsamota/Holiday.git';
                                                               }
                                                }
                 stage('TESTING') {
                                                   steps {
                                                                   echo "this is my testing stage";
                                                               }
                                              }
                 stage('QA') {
                                                   steps {
                                                                    echo "testing has been performed";
                                                              }
                                        }
                 stage('DEPLOY') {
                                                   steps {
                                                                   echo "deployement has been done on servers";
                                                               }
                                                 }
                          }
                  post {
                                always {
                                                   echo "this will always give message to developer"
                                               }
                               success {
                                                   echo "my pipeline is successfull"
                                               }
                               failure {
                                                  echo "pipeline has failed"
                                              }
                               unstable {
                                                 echo "pipeline is unstable"
                                                  }
                               changed {
                                                  echo "this will run only if the state of the pipeline or your jobs is changed"
                                                 }
                            }

           }                   
