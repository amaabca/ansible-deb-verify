Package Integrity
=================

Verify the Debian package integrity across all hosts. This role is essentially
equivalent to executing the following commands:

```bash
sudo apt-get install debsums -y
sudo debsums -s
```

See the [manpage](http://manpages.ubuntu.com/manpages/trusty/man1/debsums.1.html) for more details on operation.

Requirements
------------

This role requires the Ansible APT module.


Role Variables
--------------

This role accepts no variables.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
  - hosts: servers
    roles:
       - { role: amaabca.deb-verify }
```

License
-------

MIT

Author Information
------------------

Built by the web team at [AMA](https://ama.ab.ca) - https://github.com/amaabca.
