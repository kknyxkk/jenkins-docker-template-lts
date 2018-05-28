# Description
Template Jenkins LTS 2.107.3
user:admin
pass:admin123

# Docker build
docker build --tag smsantana/jenkins:2.107.3 --no-cache .

# Docker run
docker run --name jenkins \
    -d \
    -p 8080:8080 \
    -v jenkins_home:/var/jenkins_home \
    -v jenkins_backup:/srv/backup \
    smsantana/jenkins:2.107.3
    
    
# Optional Get Plugin in Stance Jenkins running
https://github.com/smsantana/JenkinsGetPluginApi
