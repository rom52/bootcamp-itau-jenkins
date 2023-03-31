pipeline {
    agent any;
    stages {
        stage('Listar arquivos do repositorio') {
            when {
                branch "aula-bootcamp"
            }
            steps {
                sh "ls -la"
            }
        }
        stage('GET na API do catfact') {
            when {
                branch "aula-bootcamp"
            }
            steps {
                sh "crl -XGET https://catfact.ninja/facts"
            }
        }
    }
}