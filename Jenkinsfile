pipeline {
    agent any
 stages {
     

      stage('Get Repo') {
            steps {
                sh 'sudo rm -r /var/jenkins_home/workspace/mysimpleproject/*'
                git branch: 'main', url: 'https://github.com/aliamedioune/theti'           
            }
        }     
<<<<<<< HEAD
    
=======
    stage('old build down') {
            steps {
               sh 'sudo chmod 777 -R /var/run/docker.sock'
               sh 'sudo chmod 777 -R /var/jenkins_home/workspace/mysimpleproject/'
               sh 'cd /var/jenkins_home/workspace/mysimpleproject/docker && docker compose down'
            }
        }
>>>>>>> ad306713e070190cef335d91b6f4add452da5c19
   

        
    stage('Build UP') {
            steps {
<<<<<<< HEAD
               sh 'docker build -t theti .' 
=======
               sh 'cd /var/jenkins_home/workspace/mysimpleproject/docker && docker compose up -d --build' 
>>>>>>> ad306713e070190cef335d91b6f4add452da5c19
            }
        }
    stage('Test') {
            steps {
               sh 'cd /var/jenkins_home/workspace/mysimpleproject && phpunit --log-junit result.xml UnitTestFiles/Test/'
            }
        }

    }
}
