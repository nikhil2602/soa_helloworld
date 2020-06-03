pipeline {
   agent any
 
   stages {
      stage('Build') {
         steps {
            // Get some code from a GitHub repository
            git 'https://github.com/nikhil2602/soa_helloworld.git/'
            // Run Maven on a Unix agent.
           // sh "mvn -Dmaven.test.failure.ignore=true clean package"
            // To run Maven on a Windows agent, use
             //bat "mvn pre-integration-test -f ./OSBProject1 -DoracleServerUrl=http://localhost:7101/  -DoracleUsername=weblogic -DoraclePassword=welcome1 -DoracleHome=C:/Oracle/Middleware/Oracle_Home"
            println("working");
            bat  "git pull origin master"
            bat  "git add groovy_assignment.txt"
            bat  "git commit -m \"added\""
            bat  "git push -f origin master"
            //bat "git clone'https://github.com/nikhil2602/soa_helloworld.git/'"
         }
        //post {
            // If Maven was able to run the tests, even if some of the test
            // failed, record the test results and archive the jar file.
           // success {
              // junit '**/target/surefire-reports/TEST-*.xml'
             //  archiveArtifacts 'target/*.jar'
           // }
        // }
      }
   }
}
