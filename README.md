
### Ansible Framework to bootstrap a Mac

Got a new Mac Mini but not really in the mood to do a ton of manual application install.

### Instructions

Use at your own risk there is alot of applications being installed and changes being made !!!!


#### Bootstrap dependancies

- Clone this repo 
- From terminal cd in main repo folder and run `chmod 700 && ./bootstrap.sh`
  This will simply install ruby / git / pip / ansible.


#### Review Ansible and associated code and logic.

 - From terminal `ansible --version` and ensure you get a version and no errors.

 - This repo does essentially two things, installs applications and sets up my two main development tools namely vscode and ohmyzsh.

 - The rules and code to install applications is in the playbooks folder you can amend these files as needed.

  - The rules and code to install and setup vscode and ohmyzsh are also in the playbooks folder you can amend these files as needed.


#### Run main Ansible Playbooks

There are two main wrapper Ansible main playbook in this repo. Once that contains tasks that need sudo and one that does not need sudo.

Run these with:

`sudo ansible-playbook sudo-mainplaybook.yml`
`ansible-playbook mainplaybook.yml`







sudo ansible-playbook sudo-main_playbook.yaml
ansible-playbook main_playbook.yaml

