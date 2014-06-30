# Example Project

This is an example project to boostrap buildbox agents using ansible.

```
ansible-playbook ci-agents-build.yml -i agents -vvvv
```

# Overview

So firstly I create a droplet using the digital ocean admin interface, then add this to the `agents` inventory file.

Then I retrieve and update the agent id for that host in the `ci-agents-build.yml`, if you have more than one you will need a block per agent.

# Bootstrap

The intent of this project is to illustrate how the build environment
can be boostrapped independent of buildbox, hence the bootstrap.sh being
empty in the ansible buildbox role it uses.

So with this in mind I have added a couple of example "bootstrap" build
environment recipes to the example.

# License

Copyright (c) 2014 Mark Wolfe
Licensed under the MIT license.
