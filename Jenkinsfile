 node {
     git poll: true, url:'https://github.com/eeeclipse/hello-docker.git'
  
     stage('Clone repository') {
         checkout scm 
         #repository를 jenkins workspace로 clone
     }

     stage('Build image') {
         app = docker.build("eeeclipse/jenkins:$BUILD_NUMBER") 
         #docker image build 및 이름을 eeeclipse/jenkins:빌드번호 설정
     }
}
