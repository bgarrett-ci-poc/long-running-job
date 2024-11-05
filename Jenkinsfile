pipeline {
    agent { label 'default' }
    stages {
        stage('Long running job') {
            steps {
                sh '''
                env | sort
                for i in 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20
                do
                  echo "Long running job loop #$i"
                  date
                  sleep 10s
                done
                '''
            }
        }
    }
}
