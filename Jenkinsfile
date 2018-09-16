node {
    stage('checkout') {
        checkout([$class: 'GitSCM', branches: [[name: '*/develop']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/jamesdehart/spring-petclinic.git']]])
    }
    stage ('build') {
        sh 'mvn clean install'
    }
}
