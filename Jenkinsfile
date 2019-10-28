pipeline {
	agent any
	stages {
		stage('Uploading to AWS.') {
			steps {
                    		withAWS(profile:'myProfile') {
                        	s3Upload(file:'index.html', bucket:'sagar-udacity-project-3', path:'index.html')
                    			}
			}
		}
	}
}
