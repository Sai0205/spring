pipeline{

    agent any

    stages{
        stage('Run on Coreect Slave'){
            when {
                anyOf {
                    branch 'main'
                    branch 'feature'
                }
            }
            agent {
                label "${env.BRANCH_NAME == 'main' ? 'prod' : 'dev'}"
            }
            steps {
                echo "Running on branch: ${env.BRANCH_NAME}"
                echo "Running on agent: ${env.NODE_NAME}"
            }
        }
        // stage(checkout){
        //     steps{
        //         echo "code checkout"
        //         sh "pwd"
        //         sh "ls"
        //         checkout scm
        //     }
        // }
        // stage(checkouts){
        //     steps{
        //         sh 'pwd'
        //         sh 'ls'
        //         git url: 'https://github.com/Sai0205/spring.git' , branch: 'feature'
        //         sh 'pwd'
        //         sh 'ls'
        //     }
        // }
        // stage{'checkout'}{
            
        // }
    }
}



