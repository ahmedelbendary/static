pipeline{
     agent any
     stages {
         stage('Upload to AWS') {
              steps {
                   withAWS(credentials:'aws-static') {
                      // do something
                        sh 'aws s3 ls;'
                        s3Upload(file:'index.html', bucket:'udacity-third-project', path:'./index.html')
                   }
                }
            }
         }
    }            
                 
