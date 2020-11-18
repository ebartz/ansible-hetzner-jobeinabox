
# Description

Ansible Playbook that will create a Jobeinabox with a defined count of workers.

Before you start make sure to create the `group_vars/servers.yml` from the `server.yaml.example` file.

To run this, you need to do something like this:


# Requirements

* Install Ansible 2.8 or newer
* Install required Python modules (`go to folder root and execute pip install -r pyrequirements.txt`)
* Enable hcloud inventory in Ansible configuration (explained [here](https://docs.ansible.com/ansible/latest/plugins/inventory.html))

# Usage
## Install Hetzner environment
### Spawn Env at Hetzner

```
export HCLOUD_TOKEN=hetzner-token-goes-here
ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook -i hcloud.yml site.yml
```

