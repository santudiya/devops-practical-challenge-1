Ec2 Instnaces

18.223.252.73  

ansibleuser/ansible


#################
by using ansibleuser anyone can login to above mentioned ec2 instance , for your convience  kept simple password.
In /etc all yaml and scripts are there
below are the screenshots which i took lively while doing.


#####################

- Created one Ec2 Medium instance because for installing kubectl we required minimum 2 CPUS
- on top i installed docker and kubectl
- then i started minikube driver as docker 
- create one deployment yaml to run nginx pods ( /etc/nginx.yaml)
- wrote one shell script to call the deployment file ( /etc/start_container.sh)
- now i wrote ansible playbook where it will call the start_container.sh script by using that script kubectl apply -f ngnix.yaml will trigger and nginx created.
- Monitor_container.sh will monitor the pods running status and it was scheduled in crontab.


