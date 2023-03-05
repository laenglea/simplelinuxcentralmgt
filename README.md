# Central administration template

This is a basic template to centralize the Linux Administration with ansible-pull

## Requirements

go install the required packages on the client-machines:

### Var 1 - from a ansible management machine
    
    ansible-playbook deployansible.yml --ask-pass -i 172.16.80.35,

### Var 2 - directly on the target machine

    dnf -y install epel-release && dnf -y install git ansible && dnf -y update && reboot

## Pull request

just execute

    ansible-pull -U https://github.com/laenglea/simplelinuxcentralmgt.git -i hosts
