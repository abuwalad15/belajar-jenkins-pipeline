pipeline {
    agent {
        node {
            label "linux && java21"
        }
    }
    stages {
        stage("Build") {
            steps {
                echo ("Hello Build")
            }
        }

        stage("Test") {
            steps {
                echo ("Hello Test")
            }
        }

        stage("Deploy") {
            steps {
                echo ("Hello Deploy")
            }
        }
    }
        post {
            always {
                echo "Saya akan selalu berkata Hello lagi"
            }
            success {
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
