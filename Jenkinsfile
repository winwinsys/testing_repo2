#!groovy

node {

echo "Hello from jenkinsfile"
    stage('preparation') {
        // Checkout the master branch of the hello world repository
        git branch: 'master', url: 'https://github.com/winwinsys/testing_repo2.git'
    }
    stage("compile") {
        // Run 'make` as a shell script
        sh 'make all'
    }
    stage("run") {
        // Run hello 
        sh './hello'
    }
}
