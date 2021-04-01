node {
        stage ( 'SCM' ) {
                // git clone
                git 'https://github.com/sandeep-ops/testing.git'
        }

        stage ( 'build the packages' ) {
                // mvn package
                sh 'mvn package'

        }

        stage ('archival') {
                //archiving artifacts
                archieve 'target/*.jar
        }
}
