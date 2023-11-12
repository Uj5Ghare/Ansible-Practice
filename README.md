# Ansible-Practice
This is simple Ansible project which perform following tasks......
1. Install & configure docker & start docker engine
2. Pull image from docker Hub
3. Remove existing docker container with same port
4. Create docker container which contain out application Image 
5. Start the docker container in port 5000
 

## Requirements
1. Docker (client server/machine)
  ```
  yum install docker (Amazon Linux/fedora/CentOS)
  apt install docker.io (Ubuntu/Debian)
  ```

2. Ansible  (host server/machine)
  ```
  yum install ansible (Amazon Linux/fedora/CentOS)
  apt install ansible (Ubuntu/Debian)
  ```
  IMP => You have to create "Inventory" and "ansible.cfg" file by runnig following commands 
  because above command does not create these files by default.
  ```
  mkdir /etc/ansible/
  vi /etc/ansible/hosts
  ansible-config --disabled > /etc/ansible/ansible.cfg 
  ```

## Installation
1. Clone the repository
  ```
  https://github.com/Ujwal-s-Projects/Ansible-Practice.git
  ```

2. Enter into main directory
  ```
  cd Ansible-Project/
  ```

3. Run the app [ This command will create docker container in client server node ] 
  ```
  Ansible-playbook playbook.yml
  ```
  IMP => If you are using EC2 Instance/Azure Virtual Machine then open port 5000 in security group 

4. Copy Client Server`s Public IP and paste it in browser and attach port 5000
  ```
  http://<public_ip>:5000
  ```

 
