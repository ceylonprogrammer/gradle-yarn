
pipeline{
    agent any
    
    tools{
        gradle 'Gradle-6.9'
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
                sh 'ls /var/jenkins_home/tools/hudson.plugins.gradle.GradleInstallation/Gradle-6.9'
             
               
            }
        }
        
       
    }
}
