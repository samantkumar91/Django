pipeline {
    
    agent any
    
    parameters {
        booleanParam(name: "RELEASE", defaultValue: false)
    }
    
    stages {

        stage("Build") {
            steps {
                echo "build code"
            }
        }
        
        stage("Publish") {
            steps {
                script {
                    if (params.RELEASE) {
                        echo "release"
                    } else {
                        echo "pre-release activites"
                    }
                }
            }
        }
    }
}
