# Ansible Playbook for Deploying an HAproxy Web Traffic Load Balancing
This is ansible playbook that is encrypted with ansible-vault. It can be used to run a load balancing scenario with a simple flask web application.

## How To Use It?
For running this ansible playbook you should install ansible and run lab environment from [here](https://github.com/amirhne/flask-haproxy-scenario-lab) on your machine then run following command in project root directory:
```
ansible-playbook -i inventory site.yml --ask-vault-pass
```
then enter the vault pass that is given in next part. you can see the results on your machine by entering http://127.0.0.1:8080 in your browser.

## Playbook password and Ansible Nodes Credentials
ansible-vault password: 1234567

.

loadbalancer group:

ansible@127.0.0.1:22

.

flask_servers group:

ansible@127.0.0.1:23

ansible@127.0.0.1:24

.

all servers password: 1234567

## Scenario
The Scenario is this:

![Scenario Pic](https://github.com/amirhne/flask-haproxy-scenario-playbook/blob/master/Ansible_HAProxy_Scenario.jpg)
