@Library("Demo") _
pipeline {
    agent any
    
    tools{
    maven 'maven3.9.2'

}


    stages {
        stage('git repo') {
            steps {
                gitrepo()
            }
        }
        stage('Buid'){
            steps{
                Mavenbuild()
            }
        }  
        stage('output'){
            steps{
                helloWorld()
            }
        }
    }
}
