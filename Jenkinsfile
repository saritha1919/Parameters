properties([parameters([choice(choices: ['greeting', 'silence'], description: '', name: 'REQUESTED_ACTION')])])
pipeline {
    agent any
   
  stages {
        stage ('Speak') {
            when {
                // Only say hello if a "greeting" is requested
                expression { params.REQUESTED_ACTION == 'greeting' }
            }
            steps {
                echo "Hello, bitwiseman!"
            }
        }
    }
}
