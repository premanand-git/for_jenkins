pipeline{
    agent {
        label 'master'
    }
    stages{
        stage('Parallel Stages'){
            parallel{
                stage('First Stage'){
                    steps{
                        echo "Hi, welcome to First Stage"
                    }
                }
                stage('Second Stage'){
                    steps{
                        echo "Hi, welcome to Second Stage"
                    }
                }
                stage('Third Stage'){
                    steps{
                        echo "Hi, welcome to Third Stage"
                    }
                }
            }
        }
        stage('firststage') {
            steps {
                echo 'My first pipeline with stages'
                sh """touch Prem.text"""
            }
        }
        stage('secondstage') {
            steps {
                echo 'second pipeline stage'
            }
        }
    }
}
