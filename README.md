# configuration-management-with-ansible

configuration management is a way how devops engineer configure the servers or configuration of the Infrastructure. 

Before ansible tool

suppose you are system administrator in an organisation using on on premises servers which means the organisation has its own data centers.Lets say u have bunch of servers on the data centers.suppose 20 servers hosted on linux,50 on centos etc.

He  should manages the all these servers that means he needs to upgrade,secure patches,installations on the servers.

To do it on 100's of servers like log into the servers, every time u need to update,and do installations it is very difficult even u are team of 5 members it is very difficult to manage the servers.

They use to write some scripts.If it is linux box they used to write shell scripting.If it is centos,ubuntu the commands must change.Even after writting shell scrpts these scripts should loop over like 100's of servers and execute shell commands installing and updating the packages.so it is technically very difficult to system admin doing on premises.

So,afer that entire configuration moved to cloud.with cloud the numbers of servers count increased.after moving to micro server architecture the numbers of servers has increased and also the server size but the thing is configuration of resources has decreased.

So,there was a need to find a solution to solve this problem.

To solve this problem there was a need of configuration management concept

The tools in configuration management are:

1.   puppet

2.   chef

3.   ansible

4.   salt

Among these the most used by devops engineer is ansible.  

#Ansible:

1.It is a push mechanism model.
suppose you are devops engineer u needs to create 10 EC2 instances on aws and manage the configurations like upgrade etc.here he write the  ansible scripts in ansible playbook and push the configurations to 10ec2 instances. all that he wants to do is to execute the scripts in playbook in push mechanism.

2. Agentless.
 
  1. which means it just puts the names the servers in a file called inventory file.just put the public ipadress of the server in inventory file and enable the password less authentication.
  
  2. dynamic inventory-It will auto-detect the inventory file whenever a new ec2 instance is created by xyz person and that will be managed by ansible along with existing ec2 instances.

3. pretty good with windows,linux.

4. simple(yaml)

5. we can write our own ansible modules in python.lets say u have an application like nginx load balancer.Definately u have to write the ansible modules like installing load balancer,deleting configurations.anybody else in other organisation in devops role u can share them using ansible galaxy and can use these modules and they can configure the load balancer. 

puppet:

1.  pull mechanism model

2.  master/slave architecture

3.  puppet language

 Disadvantages of ansible:

1.  configuration management with windows is not similar to linux.It is slightly difficult with windows even it has advanced modules in ansible.

2.  debugging

3.  performance








