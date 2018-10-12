pipeline {
        agent { docker { image 'php' } }
        stages {
                stage('build') {
                        steps {
                                sh 'php --version'
                        }
                }
                stage('another') {
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
