pipeline {
        agent {
              label {
                    label 'built-in'
                    customWorkspace '/data/project/vel-app'
}
}

stages{
        stage ('install-apache') {
                  steps {
                            sh 'yum install httpd -y'
                            sh 'service httpd start'
}
}
stage ('server-start') {
                    steps {
                        sh 'cp -r index.html /var/www/html'
                        sh 'chmod -R 777 /var/www/html/index.html'

}
}
}

}
