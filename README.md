# Travel Memory

####  1.Backend Configuration:
##### Clone the repository into local from https://github.com/UnpredictablePrashant/TravelMemory.
##### Kindly have a look into below screenshot for repository tree.
 ![image](https://github.com/himani0550/TravelMemory/assets/77041503/020dfa0a-7f91-4506-943e-4365a84d7570)


##### Command used to setup proxy server:
##### •	sudo apt-get update
##### •	sudo apt-get install nginx -y
##### •	sudo apt-get install nginx -y
##### •	sudo systemctl start nginx
##### •	sudo systemctl enable nginx
##### •	sudo systemctl status nginx
##### •	sudo unlink /etc/nginx/sites-enabled/default
##### •	cd /etc/nginx/sites-available/
##### •	sudo vi custom_server.conf
server {
listen 80;
location / {
proxy_pass http://my_server;
}
}
##### •	ln -s /etc/nginx/sites-available/custom_server.conf /etc/nginx/sites-enabled/custom_server.conf
##### •	sudo service nginx configtest
##### •	sudo service nginx restart

#### 2.	Frontend and Backend communication:
##### •	Updated port details in url.js file to run application on port 3000.
##### •	Frontend is running on port 80 and reverse proxy is working fine.
##### •	![image](https://github.com/himani0550/TravelMemory/assets/77041503/20b8a6c3-7526-420a-b6d1-393aa1ca8074)
##### •	Frontend and backend both is communicating with each other. Kindly refer to below screenshot.
##### •	![image](https://github.com/himani0550/TravelMemory/assets/77041503/5833b980-4ba6-4f05-938d-baf746711209)
##### •	Trip details got saved successfully to database. Kindly refer below screenshot.
##### •	![image](https://github.com/himani0550/TravelMemory/assets/77041503/0a08d28e-1f66-4264-a6e7-2f3658196d1d)
##### •	![image](https://github.com/himani0550/TravelMemory/assets/77041503/3ad44c3b-6059-4a3a-8c73-85ce1770eebb)
##### •	Loadbalancers
##### • ![image](https://github.com/himani0550/TravelMemory/assets/77041503/2e849e7e-7ae8-4c74-89b6-82b75bf12d0a)
##### • ![image](https://github.com/himani0550/TravelMemory/assets/77041503/e2750d2e-80b0-4f92-b692-d7ea87d0c63b)
##### • ![image](https://github.com/himani0550/TravelMemory/assets/77041503/eea83cbe-5cc0-4480-a00b-07212adff841)


