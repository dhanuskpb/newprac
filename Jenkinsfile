pipeline {
    agent any
    tools {
           maven "MAVEN3"
           jdk "OracleJDK8"
    }

environment{
    SNAP_REPO = 'vprofile-snapshot'
    NEXUS_USER = 'admine'
    NEXUS_PASS = 'a2725f99-76d1-43f0-b961-ac553991f582'
    RELEASE_REPO = 'vprofile-release'
    CENTRAL_REPO = 'vpro-maven-central'
    NEXUSIP = '172.31.45.82'
    NEXUSPORT = '8081'
    NEXUS_GRP_REPO = 'vpro-maven-group'
    NEXUS_LOGIN = 'nexcuslogin'
}
    stages {
        stage('build'){
            steps {
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
    stages {}
}