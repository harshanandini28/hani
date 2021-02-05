1. Enable the Deployment Manager and Compute Engine APIs.

2. In cloud shell Configure the gcloud command-line tool to use your project.
gcloud config set project [MY_PROJECT]

3. Define your resources in vm.yaml
 
4. Deploy the resources
gcloud deployment-manager deployments create quickstart-deployment --config vm.yaml

5. create custom vpc networks with subnets and configure firewalls

6. configure ssh to your vm

7. Install Nginix on VM
    sudo apt install nginx
    
  Configure UFW/Firewall for Nginx
     sudo apt install ufw
     
  Allow connections to SSH and the ports for Nginx
    sudo ufw allow ssh
    sudo ufw allow 'Nginx Full'
    sudo nano var/www/html/index.nginx.debian.html
    
    Enable UFW
     sudo ufw enable
8.  View application by using External IP Address
