This repos is responsible for cinfuguring the Jenkins cluster and it's dependent software.

As part of this ansible playbook we install java, maven and docker inside slave node. Docker and docker compose inside master node.

Also there is another playbook called jenkins_install_playbook which creates container for the jenkins and nginx.
Below are the steps to execute the ansible playbook.

Please make sure inventory has updated with master and slave IPs.

1. ansible-playbook -i inventory setup_playbook_ubunty.yml
2. ansible-playbook -i inventory jenkins_install_playbook.yml

