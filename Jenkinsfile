pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c PES1UG20CS572.cpp'
                sh 'g++ -o PES1UG20CS572 PES1UG20CS572.cpp'
                echo 'Step 1: Build stage executed successfully'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS572'
                echo 'Step 2: Test stage executed successfully'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Step 3: Deploy stage executed successfully'
            }
        }
    }
    post{
        failure{
            echo 'Failure in pipeline execution'
        }
    }
}
