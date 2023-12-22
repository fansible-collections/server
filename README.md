# Ansible Collection - mrbrandao.server

This collection aims to hold a mixed set of roles and plugins enabling the
deployment and automation for multiple GNU/Linux services.  

Such as deploy or create standalone servers, homelab servers, filesharing
servers, DNS services, kubernetes clusters.  

My initial intention on creating this is follow the new Ansible GalaxyNG
standards while also maintaining my multiple services of my interest. Such as
deploy my homelab samba server, of create my NFS shares etc...  

This collection is designed to also keep retro-compability with standalone
ansible roles, by using git submodules. Each role or plugin is maintained in a
independent git repository.


#### Installing:  

* Manual install from git URI:  
```bash
ansible-galaxy collection install mrbrandao.server
```
  
* Installing via requirements from galaxy:  

```yaml
# requirements.yml
---
collections:
  - name: mrbrandao.server
    version: 0.1.0
```

```bash
ansible-galaxy collection install -r requirements.yml -p collections/
```

#### Building the Collection:  

```bash
ansible-galaxy collection build
```

* Cloning the latest `development` version:  

```bash
git clone --recurse-submodule https://github.com/mrbrandao/server
```

#### Collection Roles:

TDB

License
-------

[GPL-2.0-or-later](https://spdx.org/licenses/GPL-2.0-or-later.html)

Author Information
------------------

Igor Brandão <@mrbrandao>
