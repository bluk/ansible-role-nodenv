ansible-role-nodenv
=========

An [Ansible](https://www.ansible.com) role to install [nodenv](https://github.com/nodenv/nodenv).

Requirements
------------

Add `nodenv` to your `$PATH` after install.

```
echo 'export PATH="$HOME/.nodenv/bin:$PATH"' >> ~/.bash_profile
```

Role Variables
--------------

* `nodenv_install_path` - The path to install `nodenv`.

* `nodenv_git_url` - The git URL to clone `nodenv` from.

* `nodenv_git_update` - If the cloned `nodenv` git repository should be updated.

* `nodenv_build_git_url` - The path to the `node-build` plugin for `nodenv`.

* `nodenv_build_git_udpate` - If the cloned `node-build` git repository should be updated.

Dependencies
------------

No dependencies.

Example Playbook
----------------

```
- hosts: servers
  roles:
     - { role: bluk.nodenv }
```

License
-------

Apache 2.0
