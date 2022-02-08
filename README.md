ECGALAXY vscode role
====================

Installs Visual Studio Code and extensions - https://code.visualstudio.com/

Requirements
------------

See https://code.visualstudio.com/docs/supporting/requirements

Role Variables
--------------

* vscode_mirror: the package repositories base URL
* vscode_extensions: the list of extensions to be installed (default: empty)
* vscode_user: vscode end user.

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

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

ECGALAXY team.
