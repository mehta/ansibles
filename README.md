lamp!
=====

ansible playbook which lamps my work environment.

Usage
-----
Ways to use ansible-command line

to apply all rules (if your ssh-user is a password-less sudoer):

    ansible-playbook -i hosts site.yml

to apply all rules (if doing ssh needs password):

    ansible-playbook -i hosts site.yml --ask-sudo-pass

to apply selective rules (eg. security):

    ansible-playbook -i hosts site.yml -l '&security'

to apply selective rules, to selective node (eg. security/nodeX):

    ansible-playbook -i hosts site.yml -l '&security:nodeX'

Thats all of it! Good to go!

IMPORTANT NOTES (Recommendations)
-------
 - ..not as of yet! :)


Ansible
------

Not sure what Ansible is? Read the getting started here: http://procbits.com/2013/09/08/getting-started-with-ansible-digital-ocean


Future RoadMap
----
- .. nothing yet!

Authors
-------
- **Abhinav Mehta**

License
-------
GPL