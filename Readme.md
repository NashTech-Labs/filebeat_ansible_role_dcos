### What will this role do ?

The above ansible role will install dcos-journalctl-filebeat service on master as well as dcos-journalctl-filebeat target on master.

The filebeat role defined above is for the master node that would be in dcos and it would serve the purpose.

So in the role script first it will create a log directory and then further will install and enable filebeat service on master node of dcos.

#### Variable used in the defaults/main.yml.

- private_deployment: '' : - This variable will be used to store the type of deployment.


### How to run the playbook .

To run the playbook follow the below command:-

`ansible-playbook -i <your inventory file> playbook.yml`

**Note**:-  If you are running on your local system then you don't need to pass inventory file. Just use localhost in hosts of playbook. 