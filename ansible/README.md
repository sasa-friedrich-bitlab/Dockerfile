# Docker image for Ansible
Docker image for `ansible` based off of `ubuntu:20.04` image.

To pull this image use:
```
docker pull fridobit/ansible
```

## Usage
### ansible-playbook

Default entrypoint in this image is `ansible-playbook`.
The best way to run this image in Linux is to set some sort of shell alias. For example bash alias:
```
alias ansible-playbook='sudo docker run -it --rm --volume $(pwd):/ansible --volume ~/.ssh/id_rsa:/root/.ssh/id_rsa:ro fridobit/ansible'
```
With such alias `ansible-playbook` command can be used as if it's installed locally on computer.