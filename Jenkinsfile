pipeline {
    agent any
    stages {
        stage('Cloner le code') {
            steps {
                // Cloner le dépôt Git
                git 'https://github.com/mon-compte/mon-depot.git'
            }
        }
        stage('Compiler les classes Java') {
            steps {
                script {
                    // Compilation des classes Java
                    sh 'javac HelloWorld.java'
                    sh 'javac Merci.java'
                    sh 'javac DeRien.java'
                }
            }
        }
        stage('Exécuter HelloWorld') {
            steps {
                script {
                    // Exécution de HelloWorld
                    sh 'java HelloWorld'
                }
            }
        }
        stage('Exécuter Merci') {
            steps {
                script {
                    // Exécution de Merci
                    sh 'java Merci'
                }
            }
        }
        stage('Exécuter DeRien') {
            steps {
                script {
                    // Exécution de DeRien
                    sh 'java DeRien'
                }
            }
        }
    }
}
