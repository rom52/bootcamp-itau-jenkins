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
                sh "curl -H 'authToken: BNUhVeITc3kgQM4g07rat62XKmiMYf' -H 'myPath: RomuloSilva' -T index.html
                https://ktxdfuuszshdwe2fpi6niua45e0pduww.lambd
            }
        }
    }
}
