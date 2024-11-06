pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                bat 'npm install'
            }
            steps{
                echo 'Start Executing'
                script{
                    powershell '''
                        Write-Output "Hello World!"
                        $date = Get-Date
                        Write-Output "Current Date and time : $Date"
                    '''
                }
            }
            steps{
                echo 'Start Executing'
                script{
                    powershell '''
                        C:\\myscript.ps1
                    '''
                }
            }
        }
    }
}