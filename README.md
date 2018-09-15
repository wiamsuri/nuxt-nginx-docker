# Nuxt.js NGINX Docker

## Getting you instance ready for Docker
With Ubuntu
```
sudo apt update
sudo apt install -y docker.io git
sudo usermod -a -G docker ubuntu
sudo service docker start
sudo curl -L https://github.com/docker/compose/releases/download/1.22.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```
or with Amazon Linux
```
#!/bin/bash
sudo yum -y update
sudo yum install -y docker git
sudo usermod -a -G docker ec2-user
sudo service docker start
sudo curl -L https://github.com/docker/compose/releases/download/1.22.0/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

## Build and run
```
docker-compose build && docker-compose up -d
```
