
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
                withGradle(){
                    sh 'chmod 777 ./gradlew'
                    sh './gradlew -v'
                }
               
            }
        }
        
       
    }
}
