pipeline {
    agent any 
	
	parameters{
    string(name: 'DOCKERIMAGE', defaultValue: 'imagename', description: 'The target environment' )
    string(name: 'qapipe', defaultValue: 'dev', description: 'The target environment' )
    booleanParam(name: 'hbp_enable', defaultValue: false, description: 'Toggle this value')   
    }
	
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!' 
            }
        }
    }
}