# hadoop-deploy
deploy hadoop on a cluster


Steps
1. Reset old configs, packages etc
ansible-playbook -i inventory reset.yml -u samy -K

2. Deploy ZK
ansible-playbook  -i inventory -l mn deploy-zk.yml   -u samy -K
