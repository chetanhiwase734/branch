pipeline {
			agent {
					label{
					
					label "built-in"
					
					
				}
			}

			  stages {
			
					stage ("23Q3"){
					
							steps {
							
								sh "cd /mnt/branch/branch"
								
								sh "git checkout 23Q3"
								sh "docker run -itdp 100:80 --name 23Q3 httpd"
								sh "docker cp index.html 23Q3:/usr/local/apache2/htdocs"
								sh "docker exec 23Q3 chmod -R 777 /usr/local/apache2/htdocs/index.html"
					}
			}
		}	
}
