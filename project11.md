# INSTALL AND CONFIGURE ANSIBLE ON EC2 INSTANCE

`sudo apt update`

`sudo apt install ansible`

![Ansible-v](./images/ansible-v.PNG)

# Configure Jenkins build job to save your repository content

![Jenkins-repo](./images/Jenkins-pointing-repo.PNG)

# Configure Webhook in GitHub and set webhook to trigger ansible build

![Webhook-config](./images/Configure-webhook.PNG)

# Configure a Post-build job to save all (**) files, like you did it in Project 9

![Postbuild](./images/post-build.PNG)

# Prepare your development environment using Visual Studio Code

# In your ansible-config-mgt GitHub repository, create a new branch that will be used for development of a new feature.

# Checkout the newly created feature branch to your local machine 

![New-branch](./images/New-branch.PNG)

![Checkout-New](./images/Checkout-newbranch.PNG)

`eval "ssh-agent -s"`

`ssh-add -k Downloads/Neyomr1.pem`

`ssh-add -l`

![ssh-agent](./images/ssh-agent.PNG)

# Create dev.yml in inventory deirectory and common.yml in playbooks directory

![dev-yml](./images/dev-yml.PNG)

![common-yml](./images/common-yml.PNG)

![git-push](./images/git-push.PNG)

`cd ansible-config-mgt`

`ansible-playbook -i inventory/dev.yml playbooks/common.yml`

![ansible-playbook](./images/run-ansibleplay.PNG)

