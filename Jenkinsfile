node{
    def MHD = tool name: "maven3.8.4"
    stage('code'){
        git branch: 'development', url: 'https://github.com/team16flight/web-app.git'
    }
    stage('BUILD'){
       sh "${MHD}/bin/mvn clean package"
 
    }
    /*
    stage('deploy'){
  steps{
  deploy adapters: [tomcat7(credentialsId: 'ea96a599-3f8a-4966-b095-0f38531ae74e', path: '', url: 'http://localhost:8080/')], contextPath: null, war: '**/*.war'
}
}
stage('email'){
emailext body: '''Build is over

Acada
437212483''', recipientProviders: [developers(), requestor()], subject: 'Build', to: 'tdapp@gmail.com'
}

    */
}
