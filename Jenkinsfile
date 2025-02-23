pipeline {
    agent {
        node {
            label "linux && java21"
        }
    }
    stages {
        stage("Hello") {
            steps {
                echo ("Hello ini sedang belajar jenkins pipeline")
            }
        }

        post {
            always {
                echo "Saya akan selalu berkata Hello lagi"
            }
            sucess {
                echo "Horee sukses"
            }
            failure {
                echo "Aduh maaf gagal"
            }
            cleanup {
                echo "Tak peduli sukses atau gagal"
            }
        }
    }
}