#### Ansible playbooks for setting up Ubuntu-based Ruby development host(s)

# Includes:

* changing shell to zsh
* installing Oh-My-Zsh
* installs rvm with MRI Ruby and JRuby (which also installs Java (JDK))


# Instructions:

* Ensure you have ssh access without password (i.e. you have added the public key to root's .ssh/authorized_keys).
* ansible-playbook ansible-devhost-deploy-user.yml
* ansible-playbook ansible-devhost-setup-up-to-chsh.yml
* Add the following line using visudo: deploy  ALL=(ALL) NOPASSWD:ALL
* ansible-playbook ansible-devhost-setup-after-chsh.yml
* set rvm default: 
