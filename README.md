#[-THE MODULE/FRAMEWORK IS NOT RELEASED YET-]

# EASYXEN 

Easyxen it will be a custom Ansible Module to automatically manage VM on XEN server hypervisors.

The final release wil include the following features:

- Create/remove VM
- Reconfigure VM
- Start/stop VM
- Build templates
- Put userdata on create VM (like AWS)

Requirements:
**

Usage:
**


# Software Architecture and Idea  [DRAFT/IN_PROGRESS]

The idea is to make a completely modular software which will work as a little framework to manage XEN with Bash and/or Python.

So, all the reusable code and functions wil be put in the '/lib/basic.sh' file that will work as a container where the other modules and functions will take the 'global' functions.

Indeed, this file contain all the functions that are used across the various states of the VMs. It contain functions like:

- Is the virtual machine present?
- Is deleted?
- Give me the UUID of the virtual machine.
...

And other.


The file is written and will be extended in BASH.
Is automatically laoded at runtime from the main Ansible module script which is "/easyxen".

===========================================================================

