pipeline {
    agent any
	
	parameters{
    string(name: 'DOCKERIMAGE', defaultValue: 'imagename', description: 'The target environment' )
    string(name: 'qapipe', defaultValue: 'dev', description: 'The target environment' )
    booleanParam(name: 'hbp_enable', defaultValue: false, description: 'Toggle this value')
	choice(choices: ['ONE', 'TWO'], name: 'PARAMETER_01')
	booleanParam(defaultValue: true, description: '', name: 'BOOLEAN')
	text(defaultValue: ''' 
     this is a multi-line 
     string parameter example
     ''',
     name: 'MULTI-LINE-STRING')
    }
	
	
	
	
    stages {
        stage('Deploying kk image') {
			when { expression { params.hbp_enable } }
            steps {
				echo 'Hello world!' 
				
			}
			
        }
    }
	
	post {
        always {
			echo 'Execution done' 
                      
            }
            
  }
    
}