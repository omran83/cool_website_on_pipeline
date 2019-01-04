pipeline {
    agent any
    triggers {
        cron('* * * * *')
    }
    stages{
        stage("git clone"){
            steps{
               git 'git@github.com:omran83/webserver_with_jenkins.git'
            }         
        }
        stage("copy file to web"){
            steps{
                sh "cp -f index.html /var/www/html/index.html"
            }
        }
        stage("test"){
            steps{
                sh "echo test"
            
            }
        } 
    }
}
