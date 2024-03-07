#Install anc configure virtual machine on Virtualbox instaled on windwos. 

# VirtualBoxVM
> Playbook:
    - CreateVM.yml
> Plays:
    - HostOnlyNetwork.yml
    - VBoxVm.yml
    
> COMMANDS:
  
> VBox VM:
      - ansible-playbook -i ../inventory/hosts VBoxVm.yml -l 'local'
> VBox "host-only-network":
      - ansible-playbook -i ../inventory/hosts HostOnlyNetwork.yml -l 'local
> Both VBox "host-only-network" + "VBox VM":
      - ansible-playbook -i ../inventory/hosts CreateVm.yml -l 'local
