# Nginx as a Reverse Proxy

A reverse proxy is a server that sits between internal applications and external clients, forwarding client requests to the appropriate server. Because NGINX has a number of advanced load balancing, security, and acceleration features that most specialized applications lack, using NGINX as a reverse proxy enables us to add these features to any application.

## Using the Reverse Proxy
1. Start each of the application sample first:
cd app-sample-1
docker-compose up -d
Repeat for each application sample needed in your project.

2. Start the Nginx Proxy:
cd ..
docker-compose up -d

3. Add the domains to your /etc/hosts file:
echo "192.168.86.100 app-sample-1" >> /etc/hosts
echo "192.168.86.100 app-sample-2" >> /etc/hosts
