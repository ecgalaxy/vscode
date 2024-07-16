ECGALAXY vscode role
====================

Installs Visual Studio Code and extensions - https://code.visualstudio.com/

Requirements
------------

See https://code.visualstudio.com/docs/supporting/requirements

Role Variables
--------------

- `vscode_mirror`: the package repositories base URL
- `vscode_extensions`: the list of extensions to be installed (default: empty)
- `vscode_user`: vscode end user

Example:

```yaml
vscode_extensions:
  - fortifyvsts.fortify-extension-for-vs-code
  - ms-azuretools.vscode-docker
  - ms-vscode-remote.remote-containers
```

Dependencies
------------

- optional: ecgalaxy.bootstrap

Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.bootstrap
        - ecgalaxy.common_packages
        - ecgalaxy.vscode

One-liner
---------

    bash <(curl -s https://code.europa.eu/-/snippets/1/raw/main/ansible-role.sh) ecgalaxy.vscode

See [ansible-role](https://code.europa.eu/-/snippets/1) for instructions.

Please verify the script integrity first.

Upgrading & Uninstalling
------------------------

This Ansible role uses the distribution's package manager to install packages.

In order to upgrade or uninstall a package, please refer to your distribution's package manager documentation.

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

[ECGALAXY](https://code.europa.eu/groups/ecgalaxy/-/wikis/home) team.
