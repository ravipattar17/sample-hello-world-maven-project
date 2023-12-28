pipeline{
    agent{
        label "built-in"
    }
    stages{
        stage ("compile/sonar-scanner-analysis/deploy-to-nexus-artifact") {
            steps {
            sh "/mnt/tools/apache-maven-3.9.6/bin/mvn deploy sonar:sonar"		// compile-analysis-deploy-to-nexus-artifact
            }
        }
     
    }
}
