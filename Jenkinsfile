pipeline {
    agent any
    Parameters{
        string(name:'MAVEN_GOAL' defaultValue:'mvn clean package' decription:'mavengoal')
    }

    stages {
        stage ('get source code') {
            steps{
                git url: 'https://github.com/spring-projects/spring-petclinic.git'
                branch: 'main'
            }
        }
    }
}