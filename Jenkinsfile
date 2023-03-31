pipeline {
    agent any;
    stages {
        stage('Listar arquivos do repositorio') {
            when {
                branch "main"
            }
            steps {
                sh "ls -la"
            }
        }
        stage('PUT na API do catfact') {
            when {
                branch "main"
            }
            steps {
                $ curl -H 'authToken: BNUhVeITc3kgQM4g07rat62XKmiMYf' -H 'myPath: <seu-path>' -T index.html https://ktxdfuuszshdwe2fpi6niua45e0pduww.lambda-url.us-east-1.on.aws/
            }
        }
    }
}
