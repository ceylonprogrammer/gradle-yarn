
pipeline{
    agent any
    stages{
        stage("run front end"){
            steps{
                echo 'executing yarn '
                nodejs("Node-10.17.0"){
                    sh 'yarn install'
                }
            }
        }
        
         stage("run backend"){
            steps{
                echo 'executing gradle'
                withGradle() {
                        sh 'gradle wrapper'
                        sh 'ls -al'
                }
               
            }
        }
        
       
    }
}
