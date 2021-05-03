ECGALAXY vscode role
====================

Installs Visual Studio Code - https://code.visualstudio.com/

Requirements
------------

See https://code.visualstudio.com/docs/supporting/requirements

Role Variables
--------------

* vscode_mirror: the package repositories base URL
* vscode_extensions: the list of extensions to be installed (default: empty)

Example:

```yaml
vscode_extensions:
  - fortifyvsts.fortify-extension-for-vs-code
  - ms-azuretools.vscode-docker
  - ms-vscode-remote.remote-containers
```

Dependencies
------------

* optional: ecgalaxy.bootstrap

License
-------

EUPL-1.2

Author Information
------------------

ECGALAXY team.
