# zabbix-all-in-one
All zabbix framework running in kubernetes

# How to use
1. Download all files

1. Edit the *zabbix-all-in-one.yaml* changing all passwords (where is write 'changeme123') to something strong (or whatever do you want).

1. Perform kubectl commands:

    * Start all framework:
    
    `kubectl apply -f zabbix-all-in-one.yaml`
  
    * Check information about the services:
    
    `kubectl describe service zabbix-web`
   
   `kubectl describe service zabbix-db`
   
   `kubectl describe service zabbix-server`
 
    * Delete all services:
   
   `kubectl delete service zabbix-web`
   
   `kubectl delete service zabbix-db`
   
   `kubectl delete service zabbix-server`
   
   
   For more tips, visit the kubernetes documentation page: https://kubernetes.io/
