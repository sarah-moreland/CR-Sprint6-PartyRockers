pipeline {
    agent none
    stages {
        stage('Build') {
            steps {

               echo 'This is the build stage.'
               awsCodeBuild projectName: "${APPLICATION_NAME}-codebuild", credentialsType: 'keys', region: "${AWS_REGION}", sourceControlType: 'project', sourceVersion: "${BRANCH_NAME}"

            }
        }

        // stage('Testing') {
        //     steps {

        //        echo 'This is the test stage.'
        //     }
        // }

        // stage('E2E Testing') {
        //     steps {

        //        echo 'This is the E2E Testing stage.'
        //     }
        // }

        // stage('Deploy') {
        //     steps {

        //        echo 'This is the deploy stage.'
        //     }
        // }
    }
}