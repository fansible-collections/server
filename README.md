# Ansible Collection - fansilet.homelab

This collection aims to hold a mixed set of roles and plugins enabling the
deployment and automation for multiple GNU/Linux services.  

Such as deploy or create standalone servers, homelab servers, filesharing
servers, DNS services, kubernetes clusters.  

The initial intention on creating this is follow the new Ansible GalaxyNG
standards while also maintaining multiple services of my interest. Such as
deploy my homelab samba server, or create NFS shares etc...  

This collection is designed to also keep retro-compability with standalone
ansible roles, by using git submodules. Each role or plugin is maintained in a
independent git repository.

All roles of this collections can be found in the
[fansilet-roles](https://github.com/fansilet-roles) organization.



#### Installing:  

* Manual install from git URI:  
```bash
ansible-galaxy collection install fansilet.homelab
```
  
* Installing via requirements from galaxy:  

```yaml
# requirements.yml
---
collections:
  - name: fansilet.homelab
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
git clone --recurse-submodule https://github.com/fansilet-collections/homelab
```

* Using the [`Makefile`](Makefile):  
_alternativelly is possible to build and push the collection using the
`Makefile` e.g:_  

```bash
# build the collection
make build
```

```bash
# cleaning the built collection
make clean
```

```bash
# publish the collection to ansible-galaxy
make push
```

#### Collection Roles:

TDB

#### Q&A

Q: Why fansilet?  
A: The orignal name was fansible, in the sense of "It's Fancy, It's Ansible,
It's fansible. However this evolved to use [podman
quadlet](https://www.redhat.com/sysadmin/quadlet-podman), becoming: "It's Fancy,
It's Ansible, It's Quadlet, It's Fansilet.  

Q: Why there's two orgs in github, fansilet-collections and fansible-roles?  
A: In gitlab we have groups which allows to organize better or code. In Github
the similar way of solving it is by having orgs.  

License
-------

[GPL-2.0-or-later](https://spdx.org/licenses/GPL-2.0-or-later.html)

Author and Acknowledge
-----------------------

Igor Brandão <@mrbrandao>
