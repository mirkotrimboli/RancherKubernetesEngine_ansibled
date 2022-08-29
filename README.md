# RancherKubernetesEngine_ansibled
This playbook aims to produce an RKE in Stand Alone mode on Docker.

# Release note
* The code work on multiple Operative Systems Linux based.
* It is tested with: Ubuntu 18.04LTS, 20.04LTS, CentOS 7.x, 8.x
* It is meant for to get a Rancher Web console predisposed behind a proxy, if necessary you can enable tasks in playbook yaml file.
* It is meant for work also on Cloud on IaaS.

# To use this code:
* Download the playbook.
* Edit your hosts file with IP and hostnames of your servers.
* Edit playbook hosts file with hostnames of your servers.
* Compile file in group_vars directory as is it is explained.
* Then you must to move into the folder with command: "cd /absolute/path/to/playbook".
* Finally you can run the code with command: "ansible-playbook -i rke.hosts rke.yaml".

# For use on Cloud
* Edit playbook hosts file without references to password.
* You can run the code with command: "ansible-playbook -i rke.hosts rke.yaml --key-file=/absolute/path/to/key.pem".
