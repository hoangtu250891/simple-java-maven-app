pipeline 
{
    agent any

    stages {
        stage('Build') 
        { 
            steps 
            {
                //bat 'mvn -B -DskipTests clean package' 
                echo "${params.WORKSPACE}"
            }
        }
        stage('Test') 
        {
            steps 
            {
                bat 'mvn test'
            }

        }
    }
}
