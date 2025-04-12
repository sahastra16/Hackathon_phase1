pipeline{
    agent any;
    stages{
        stage("code"){
            steps {
                git url: "https://github.com/Swayamnakshane/Hackathon_phase1.git" , branch: "swayam_feature"
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
