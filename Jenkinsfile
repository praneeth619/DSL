node {
   
    def JAVA_HOME="%JAVA_HOME%\bin"
    def MAVEN_HOME="%MAVEN_HOME%\bin"
    stage ('Checkout') {
    git 'https://github.com/praneeth619/DevOpsClassCodes.git'    
    }
    stage ('Compile') {
        echo "compiling the code"
        script {
            bat 'call mvn compile'
        }
    }
    stage ('Package') {
        echo "packaging the code"
        script {
            bat 'call mvn package'
        }
    }
}

