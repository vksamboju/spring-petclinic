node ('MVN') {
    
    stage('GIT') {
        git branch: 'dev', url: 'https://github.com/vksamboju/spring-petclinic.git'
    }
    
    stage('Build') {
        sh 'mvn install'
    }
    stage('dummy') {
        sh 'pwd'
    }

    stage('Archive') {
        archive 'target//*.jar'
        junit 'target/surefire-reports/*.xml'
    }
}