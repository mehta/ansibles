changelog convention
-----------
**major.minor[.build[.revision]]**, where

  - **major**: changes when role is fully completed (updates only in master)
  - **minor**: changes when role is partially completed (updates only in master or develop)
  - **build**: changes when big chunk of role is written and available for build/revision or bugfixes
-----

### v0.2.2 (2014-04-28)
* bugfix: If a unix-user is logged in, than you can't modify subject settings, as a result www-data user for nginx was breaking ansible-process, so solution is to ignore editing user, if user is logged-in.

### v0.2.1 (2014-04-28)
* bugfix: In 'remove users' task of users-role, it has wrong list name, fixed!

### v0.2.0 (2014-04-28)
* change: users role working for `Debian` machines, which manages users and groups, it also manages authorized ssh-keys

### v0.1.0 (2014-04-27)
* change: common role working for `Debian` machines, which manages debian packages
* change: nginx role working for `Debian` machines, with source & package built options

### v0.0.1 (2014-04-10)
* started maintaining changelog
* change: get the base project structure and directories in right shape
