pipeline {
	agent any
	stages {
		stage('Uploading to AWS.') {
			steps {
				dir('./'){
                    		pwd();

                    		withAWS(region:'us-east-1', credentials:'aws-static') {
                        	s3Upload(file:'index.html', bucket:'sagar-project-03', path:'')
                    			}
                		}
			}
		}
	}
}
