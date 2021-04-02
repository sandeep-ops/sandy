node {
        stage ( 'SCM' ) {
                // git clone
                git 'https://github.com/sandeep-ops/sandy.git'
        }

        stage ( 'build the packages' ) {
           CheckInput =  input message: 'Please provide the envname', parameters: [choice(choices: ['1', '2'], description: 'Please select the input', name: 'Name')]
           if (CheckInput == '1'){
               
                // mvn package
                sh 'mvn package'
           }
           else{
               echo "Go and check condition"
           }
        }

}
