pipeline {
        agent any

        stages {
                stage('Hello') {
                        steps {
                                echo 'Hello World3'
                                }
                        }
                
                stage('Build') {
                agent { label 'docker-agent' }
                steps {
                        sh 'echo "Hello World"'
                        sh '''
                        echo "Multiline shell steps works too"
                        ls -lah
                        '''
                        }
                }
         }
} 
