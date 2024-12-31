pipeline {
    agent any
    tools { nodejs 'Node'}
    stages {
        stage('Petició de dades') {
            input {
                message "Introdueix nom del executor: "
                ok "Enviar"
                parameters {
                    string(name: 'EXECUTOR', defaultValue: 'usuari', description: 'nom de la persona que executa la pipeline')
                }
            }
            steps {
                echo "Benvingut ${EXECUTOR}."
            }
        }
    }
}