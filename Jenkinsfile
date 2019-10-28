pipeline {
	agent any
	stages {
		stage('Uploading to AWS.') {
			steps {
				dir('./'){
                    		pwd();

                    		withAWS(credentials:'aws-static') {
                        	s3Upload(file:'index.html', bucket:'sagar-udacity-project-3', path:'')
                    			}
                		}
			}
		}
	}
}
