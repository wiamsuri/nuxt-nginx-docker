# Nuxt.js NGINX Docker

```
#!/bin/bash
sudo yum -y update
sudo yum install -y docker
sudo usermod -a -G docker ec2-user
sudo service docker start
sudo pip install docker-compose
```
