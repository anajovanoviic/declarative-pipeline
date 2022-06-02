pipeline {

    agent any
    parameters {
        string(name: 'PERSON', defaultValue: 'Ana', description: 'Upisi ime')

        

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
    }
    
    stages {
        stage("Step 1") {
            steps {
                println('Hello ${params.PERSON}')
                if(${params.TOGGLE}){
                    echo "Status je true"
                } else {
                    echo "Status je false"
                }
            }
        }
        stage("Step 2 - Git") {
            steps {
                println('testing the applicatiojn...')
                
                }
            }
        }
        
    }   
}
