pipeline 
{
    agent any

    stages {
        stage('Build') 
        { 
            steps 
            {
                //bat 'mvn -B -DskipTests clean package' 
                echo "WORKSPACE: ${WORKSPACE}"
                echo "BRANCH_NAME: ${BRANCH_NAME}"
                echo "BUILD_NUMBER: ${BUILD_NUMBER}"
                echo "JENKINS_HOME: ${JENKINS_HOME}"
                echo "JENKINS_URL: ${JENKINS_URL}"
                echo "GIT_BRANCH: ${GIT_BRANCH}"
                echo "GIT_AUTHOR_NAME: ${GIT_AUTHOR_NAME}"
                
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
