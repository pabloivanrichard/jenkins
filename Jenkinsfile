@Library('jenkinsLibs') _
pipeline {
    agent any
parameter{
string(name:'url',description:'Url para enviar un post')
string(name:'message',description:"menssage que va al post")

}
    stages {
        stage('request api') {
            steps {
                echo "Url: ${params.url}"
                echo "Url: ${params.message}"
                apimessageSender(params.url, params.message)
              
            }
        }
      
    }
}