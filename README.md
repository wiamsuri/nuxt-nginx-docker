# Nuxt.js NGINX Docker

```
#!/bin/bash
sudo yum -y update
sudo yum install -y docker git
sudo usermod -a -G docker ec2-user
sudo service docker start
sudo pip install docker-compose
```

```
docker-compose build && docker-compose up -d
```
