
pipeline{
    agent any
    
    tools{
        gradle Gradle-6.9.3
    }
    
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
                sh 'ls -al'
                sh './gradlew -v'
             
               
            }
        }
        
       
    }
}
