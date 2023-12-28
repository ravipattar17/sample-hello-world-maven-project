pipeline{
    agent{
        label "built-in"
    }
    stages{
        stage ("compile/sonar-scanner-analysis/deploy-to-nexus-artifact") {
            steps {
            sh "mvn deploy sonar:sonar"		// compile-analysis-deploy-to-nexus-artifact
            }
        }
     
    }
}
