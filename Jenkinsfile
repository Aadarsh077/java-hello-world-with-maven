node {
    def mvnHome = tool 'MVN' 

    stage('Checkout') {
        
        git credentialsId: 'c4069d2c-72eb-4384-a106-c3609a9cbfdc', url: 'https://github.com/Aadarsh077/java-hello-world-with-maven.git'
    }

    stage('Validate') {
       
        bat "${mvnHome}\\bin\\mvn validate"
    }

    stage('Clean') {
        
        bat "${mvnHome}\\bin\\mvn clean"
    }

    stage('Compile') {
       
        bat "${mvnHome}\\bin\\mvn compile"
    }

    stage('Test') {
        
        bat "${mvnHome}\\bin\\mvn test"
    }

    stage('Package') {
       
        bat "${mvnHome}\\bin\\mvn package"
    }

    stage('Verify') {
        
        bat "${mvnHome}\\bin\\mvn verify"
    }

    stage('Install') {
        
        bat "${mvnHome}\\bin\\mvn install"
    }

    stage('Site') {
        
        bat "${mvnHome}\\bin\\mvn site"
    }
}
