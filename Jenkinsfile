 node {
     git poll: true, url:'https://github.com/eeeclipse/hello-docker.git'
  
     stage('Clone repository') {
         checkout scm 
     }

     stage('Build image') {
         app = docker.build("eeeclipse/jenkins:$BUILD_NUMBER") 
     }
}
