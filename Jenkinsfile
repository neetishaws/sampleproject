node{
  stage("Checkout SCM"){

         git credentialsId: '0a1d1b6f-022b-442a-8355-5844a4ea0069', url: 'https://github.com/neetishaws/sampleproject.git'
    }

  stage("MVN Package"){

        def mvnHome = tool name: 'Maven home', type: 'maven'
        def mvnCMD = "${mvnHome}/bin/mvn"
        sh ("${mvnCMD} clean package")
}
}

