# Example Project

This is an example project to boostrap buildbox agents using ansible.

```
ansible-playbook ci-agents-build.yml -i agents -vvvv
```

# Overview

So firstly I create a droplet using the digital ocean admin interface, then add this to the `agents` inventory file.

Then I retrieve and update the agent id for that host in the `ci-agents-build.yml`, if you have more than one you will need a block per agent.
