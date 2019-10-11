node ('MVN') {
    
    stage('GIT') {
        git branch: 'dev', url: 'https://github.com/sambojuvk/spring-petclinic.git'
    }
    
    stage('Build') {
        sh 'mvn package'
    }

    
}