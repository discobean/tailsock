def test_python()
{
    node {
        sh """
            virutalenv env
            source env/bin/activate
            pip install -r requirements.txt
        """
    }
}


pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                test_python()
            }
        }
        stage('Test'){
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}

