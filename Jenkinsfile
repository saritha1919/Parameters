properties([parameters([booleanParam(defaultValue: false, description: '', name: 'CodeAnalysis'), booleanParam(defaultValue: false, description: '', name: 'Deployment')])])
pipeline {
    agent any
   
  stages {
        stage ('Code analysis') {
            when {
                // Only say hello if a "greeting" is requested
                expression { params.CodeAnalysis == 'true' }
            }
            steps {
                echo "code analysis done."
            }
        }
    }
}
