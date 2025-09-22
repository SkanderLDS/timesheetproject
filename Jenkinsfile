pipeline {
    agent any
    tools {
        // Corrected quotes around JAVA_HOME
        jdk 'JAVA_HOME'
        maven 'M2_HOME'
    }
    stages {
        stage('GIT') {
            steps {
                git branch: 'main', url: 'https://github.com/SkanderLDS/timesheetproject.git'
            }
        }
        stage('Compile Stage') {
            steps {
                sh 'mvn clean compile'
            }
        }
    }
}
