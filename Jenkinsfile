pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                bat 'npm install'
            }
        stage('Script'){
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
        }
        stage('File'){
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
}