pipeline{
    agent {label "dev"}
    stages{
        stage("code"){
            steps {
                git url: "https://github.com/sahastra16/Hackathon_phase1.git" , branch: "dev"
            }
        }
        stage("build"){
            steps {
                sh "docker build -t onlineapp ."
            }
        }
        stage("test"){
            steps {
                echo "no test case"
            }
        }
        stage("deploy"){
            steps {
                sh "docker compose up -d"
            }
        }
    }
}
