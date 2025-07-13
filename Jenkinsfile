pipeline{

    agent any

    stages{
        stage(checkout){
            steps{
                echo "code checkout"
                sh "pwd"
                sh "ls"
                checkout scm
            }
        }
        stage(checkouts){
            steps{
                sh 'pwd'
                sh 'ls'
                git url: 'https://github.com/Sai0205/spring.git' , branch: 'main'
                sh 'pwd'
                sh 'ls'
            }
        }

    }
}



