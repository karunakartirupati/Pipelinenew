pipeline {
    agent any {
	}
	parameters{
    string(name: 'DOCKERIMAGE', defaultValue: 'imagename', description: 'The target environment' )
    string(name: 'qapipe', defaultValue: 'dev', description: 'The target environment' )
    booleanParam(name: 'hbp_enable', defaultValue: false, description: 'Toggle this value')   
    }
	
	
	
    stages {
        stage('Deploying kk image') {
			when { expression { params.hbp_enable } }
            steps {
				dir ('/c/Users/tirupati/pipelinenew'){
					echo 'Inside repo'
				}			
				echo 'Hello world!' 
			}
			
        }
    }
    
}