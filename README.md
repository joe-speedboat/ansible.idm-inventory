# ansible.idm-inventory
This is just for my personal AWX integration testing.
Not more, not less.

## HowTo use
### Create new Execution Environment
* Name: Custom EE
* Image: docker.io/christian773/ansible-ee:latest
* Description: FreeIPA Python deps + Collections
* Pull: Missing

### Create new Inventory Project
* Source Control Type: Git
* URL:     https://github.com/joe-speedboat/ansible.idm-inventory.git

### Create new Inventory Source
* Add inventory
* Add new source from project
* Inventory file: / (project root)
* Execution Environment: Custom EE
* Source variables   
   freeipaserver: ipa-server.domain.local   
   freeipauser: ipa-ro-user   
   freeipapassword: ipa-ro-password   
