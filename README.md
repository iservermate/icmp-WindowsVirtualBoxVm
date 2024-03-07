**Install anc configure virtual machine on Virtualbox instaled on windwos.**

**Playbook:**<br>
    - CreateVM.yml
**Plays:**:**<br>
    - HostOnlyNetwork.yml
    - VBoxVm.yml

**COMMANDS:**:**<br>
  
**VBox VM:**
    - ansible-playbook -i ../inventory/hosts VBoxVm.yml -l 'local'
 
**VBox "host-only-network":**
    - ansible-playbook -i ../inventory/hosts HostOnlyNetwork.yml -l 'local
 
**Both VBox "host-only-network" + "VBox VM":**
    - ansible-playbook -i ../inventory/hosts CreateVm.yml -l 'local
