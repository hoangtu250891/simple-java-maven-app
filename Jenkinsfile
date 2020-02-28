pipeline 
{
    agent any

    stages {
        stage('Build') 
        { 
            steps 
            {
                //bat 'mvn -B -DskipTests clean package' 
                echo "${WORKSPACE}"
                echo "${WORKSPACE}\"
                echo "PATH = ${PATH}"
                echo "M2_HOME = ${MAVEN_HOME}"
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
