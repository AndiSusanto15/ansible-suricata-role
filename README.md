# Ansible roles install suricata ubuntu and CentOS

## Vars

```yml
suricata_sniffing_interface: #  default( ansible_default_ipv4.interface )
```

## Sample Playbook

```yml
---
- hosts: all
  become: yes
  vars:
    suricata_sniffing_interface: eth0

  roles:
    - { role: batutah.suricata }
```

## References

- https://github.com/Alir3z4/ansible-suricata/
- https://redmine.openinfosecfoundation.org/projects/suricata/wiki/Suricata_installation
- https://www.sealingtech.com/blog/adventures-in-suricata-part-1-low-cost-intrusion-detection-system/
- https://suricata.io/learn/
- https://suricata.io/features/ 
- https://launchpad.net/~oisf/+archive/ubuntu/suricata-stable
- https://www.atlantic.net/vps-hosting/how-to-install-and-setup-suricata-ids-on-ubuntu-20-04/
