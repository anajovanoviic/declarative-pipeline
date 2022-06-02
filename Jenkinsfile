pipeline {
    agent any
    stages {
        stage('Setup parameters') {
            steps {
                script { 
                    properties([
                        parameters([
                            choice(
                                choices: ['ONE', 'TWO'], 
                                name: 'PARAMETER_01'
                            ),
                            booleanParam(
                                defaultValue: true, 
                                description: '', 
                                name: 'BOOLEAN'
                            ),
                            string(
                                defaultValue: 'scriptcrunch', 
                                name: 'STRING-PARAMETER', 
                                trim: true
                            )
                        ])
                    ])
                }

                println("Hello ${params.PARAMETER_01}")

                println("Hello world")
            }
        }

 stage("Stage 2"){
            steps {
                script {
                    withCredentials([usernamePassword(credentialsId: '133b314d-d52d-4c4f-ae2f-03a051fed5a4', passwordVariable: 'password', usernameVariable: 'username')]) {
    
}{
                echo "Cloning the Repository..."
            git 'https://github.com/Fireplusplus/Project'
        }
        }
    }
}
    }   
}
