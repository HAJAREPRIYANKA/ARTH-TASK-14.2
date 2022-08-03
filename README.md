# ARTH-TASK-14.2
Create An Ansible Playbook that will Retrieve New Container IP and Update the Inventory. So further Configuration of the Webserver could be done inside that Container.

Ansible | Docker | Dynamic inventory | apache
Published on January 1, 2021

Suyog ShindeStatus is reachable
Suyog Shinde
CKA | AWS Certified Solution Architect | 2x Red Hat Certified Engineer | DevOps engineer | DevOps (Kubernetes, Docker, Openshift )| Ansible | Terraform | Cloud Computing ☁(Aws, Gcp, Azure))
20 articles 
Following
What is ansible?
No alt text provided for this image


Ansible is an open-source software provisioning, configuration management, and application-deployment tool enabling infrastructure as code. It runs on many Unix-like systems and can configure both Unix-like systems as well as Microsoft Windows.

What is Docker?
No alt text provided for this image


Docker is an application build and deployment tool. It is based on the idea that you can package your code with dependencies into a deployable unit called a container. Containers have been around for quite some time

What is Apache HTTP Server?
No alt text provided for this image


Apache HTTP Server is a free and open-source web server that delivers web content through the internet. It is commonly referred to as Apache and after development, it quickly became the most popular HTTP client on the web.

✍️✍️Task Description📄

🔰 14.2 Further in ARTH - Task 10 has to create an ansible playbook that will retrieve new container IP and update the inventory. So that further Configuration of the Webserver could be done inside that Container.

Now, Let's begin

The inventory file is empty.

No alt text provided for this image
This task is performed on localHost And this my playbook 1 docker.yml
Steps in the first playbook docker.yml
No alt text provided for this image
Using the Ansible facts we retrieved the container IP and stored it

No alt text provided for this image
Now, Running the above playbook will launch a new container and dynamically input the IP into the inventory file inv.txt.

Container Name: happynewyear

No alt text provided for this image
Container IP: 172.17.0.2

Let's check if the inventory file is updated or not.

No alt text provided for this image
It's successfully updated.

Now further, let's configure the web server on that container.
The second playbook fweb.yml
No alt text provided for this image
After running the playbook.
No alt text provided for this image
No alt text provided for this image
Successfully configured the webserver on a docker container and dynamically stored the IP in the inventory file.
Thank You !!!⭐⭐

Keep Learning !! Keep Sharing!!!⭐⭐

