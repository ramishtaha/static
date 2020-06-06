pipeline {
  agent any
  stages {
    stage('UploadtoAWS') {
      steps {
        withAWS(region:'us-west-2', credentials:'aws-static') {
          s3Upload(file:'index.html', bucket:'static-ramish', path:'https://static-ramish.s3.amazonaws.com/index.html')
        }
       }
     }
  }
}