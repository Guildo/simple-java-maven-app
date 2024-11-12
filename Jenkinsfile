pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                withMaven(maven: 'M3', mavenLocalRepo: '.repository') {
                    sh 'mvn -B -DskipTests clean package'
                }
            }
        }
    }
}