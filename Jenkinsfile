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
        stage('GET na API do catfact') {
            when {
                branch "main"
            }
            steps {
                sh "crl -XGET https://catfact.ninja/facts"
            }
        }
    }
}
