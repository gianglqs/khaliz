pipeline {
    agent any
    stages {
        
        stage('Build') {
            steps {
              echo "Hello Anh Giang hehehe"
            }
        }
    }
}


#declare params

pipeline {
    agent any
    parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
    stages {
        stage('Example') {
            steps {
                echo "${params.Greeting} World!"
            }
        }
    }
}
