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
        stage ("trigger 2nd stage") {
            steps {
            build "step2-deploy-war-ansible-to-slave1"	// has to be same name 
            }											// as I have given to 2nd stage
        }
    }
}
