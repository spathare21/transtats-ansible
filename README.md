Ansible project for Deploying Transtats


### How to use

- Install ansible on your computer (`sudo pip install ansible` should do the
  trick).
- Clone this project.
- Edit the `transtats-ansible/hosts` file and enter the IP address of the server you are
	deploying to and edit the path to the private key file.
- Run the playbook:

	```
	cd transtats-ansible
	ansible-playbook provision.yml
	```	
- Run playbook with environment variable if you want to change the db name..etc

    ```
    cd transtats-ansible
	ansible-playbook "-e 'DATABASE_NAME=db_name DATABASE_USER=db_user  DATABASE_PASSWD=db_pass  DATABASE_HOST=db_host'" provision.yml 
	``` 

	Replace the value in place of db_name, db_user, db_pass and db_host. 