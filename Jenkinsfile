pipeline {
   agent any 
   stages{
   stage('Build'){
    steps{
     sh '/Users/vigneshd/Documents/apache-maven-3.6.0/bin/mvn clean package'
     sh "echo bettaty | sudo -S"
     sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
    }
   }
   }
}
