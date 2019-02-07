pipeline {
   agent any 
   stages{
   stage('Build'){
    steps{
     sh '/Users/vigneshd/Documents/apache-maven-3.6.0/bin/mvn clean package'
     sh "/usr/local/bin/docker build . -t tomcatwebapp:${env.BUILD_ID}"
    }
   }
   }
}
