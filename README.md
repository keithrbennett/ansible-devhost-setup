#### Ansible playbooks for setting up Ubuntu-based Ruby development host(s)

Includes:

* changing shell to zsh
* installing Oh-My-Zsh
* installs rvm with MRI Ruby and JRuby (which also installs Java (JDK))

Assumes hosts are defined somewhere accessible; I have an /etc/ansible/hosts file containing this:

[devhosts]
ubuntu-vm

