pipeline {
      agent any
      stages {
            stage('Init') {
                  steps {
                        echo 'Hi, this is Ashutosh from giit'
                        echo 'We are Starting the Testing'
                  }
            }
            stage('Build') {
                  steps {
                        echo 'initializing the git repo. in httpd web server'
                        sh '''
                              sudo cd /var/www/html
                              sudo git init
                        '''
                  }
            }
            stage('Deploy') {
                  steps {
                        echo "Deploying the test website"
                        sh '''
                              sudo cd /var/www/html
                              sudo git pull git pull https://github.com/ashutoshdubey21/web-demo.git
                        '''
                  }
            }
            
      }
}
