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
                        dir('/var/www/html/') {
                              git init
                        }
                        
                  }
            }
            stage('Deploy') {
                  steps {
                        echo "Deploying the test website"
                        dir('/var/www/html/') {
                              git pull https://github.com/ashutoshdubey21/web-demo.git
                        }
                        
                  }
            }
            
      }
}
