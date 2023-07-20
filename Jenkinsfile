@Library('jenkinsLibs') _
pipeline {
    agent any
parameters{
string(name:'url',description:'Url para enviar un post')
string(name:'message',description:"menssage que va al post")

}
    stages {
        stage('request api') {
            steps {
                echo "Url: ${params.url}"
                echo "Url: ${params.message}"
                apimessageSenderLib.apimessageSender(${params.url},${params.message})
              
            }
        }
      
    }
}