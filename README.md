# Travel Memory

####  1.Backend Configuration:
##### Clone the repository into local from https://github.com/UnpredictablePrashant/TravelMemory.
##### Kindly have a look into below screenshot for repository tree.
 ![image](https://github.com/himani0550/TravelMemory/assets/77041503/020dfa0a-7f91-4506-943e-4365a84d7570)


##### Command used to setup proxy server:
•	sudo apt-get update
•	sudo apt-get install nginx -y
•	sudo apt-get install nginx -y
•	sudo systemctl start nginx
•	sudo systemctl enable nginx
•	sudo systemctl status nginx
•	sudo unlink /etc/nginx/sites-enabled/default
•	cd /etc/nginx/sites-available/
•	sudo vi custom_server.conf
server {
listen 80;
location / {
proxy_pass http://my_server;
}
}
•	ln -s /etc/nginx/sites-available/custom_server.conf /etc/nginx/sites-enabled/custom_server.conf
•	sudo service nginx configtest
•	sudo service nginx restart

#### 2.	Frontend and Backend communication:
•	Updated port details in url.js file to run application on port 3000.
•	Frontend is running on port 80 and reverse proxy is working fine.
•	
•	 
•	Frontend and backend both is communicating with each other. Kindly refer to below screenshot.
•	 

•	Trip details got saved successfully to database. Kindly refer below screenshot.
•	 
•	
 
•	Loadbalancers
•
