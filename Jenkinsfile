node ('MVN') {
    
    stage('GIT') {
        git branch: 'dev', url: 'https://github.com/sambojuvk/spring-petclinic.git'
    }
    
    stage('Build') {
        sh 'mvn package'
    }

    stage('Archive') {
        archive 'target//*.jar'
        junit 'target/surefire-reports/*.xml'
    }
}