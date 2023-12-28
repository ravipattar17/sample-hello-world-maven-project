pipeline{
    agent{
        label "built-in"
    }
    stages{
        stage ("compile/sonar-scanner-analysis/deploy-to-nexus-artifact") {
            steps {
            sh "echo 'export PATH="/mnt/tools/sonar-scanner-4.6.2.2472-linux/bin:$PATH"' >> ~/.bash_profile"
            sh "source ~/.bash_profile"
            sh 'export PATH="/mnt/tools/sonar-scanner-4.6.2.2472-linux/bin:$PATH"'
            sh "/mnt/tools/apache-maven-3.9.6/bin/mvn deploy sonar:sonar"		// compile-analysis-deploy-to-nexus-artifact
            }
        }
     
    }
}
