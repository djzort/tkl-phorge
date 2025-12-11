Phorge - an opinionated platform for collaborating, managing, organizing and reviewing software projects.
=============================================

`Phorge`_ is repository system, which succeeds Phabricator.

This appliance includes all the standard features in `TurnKey Core`_,
and on top of that:

- Phorge configurations:

    - Installed from upstream source code to /opt/phorge
    - Arcanist from upstream source code to /opt/arcanist
    - Git, SVN, and Mercurial support
    - Defaults to emailing via local mail through postfix

- SSL support out of the box.
- `Adminer`_ administration frontend for MySQL (listening on port
  12322 - uses SSL).
- Postfix MTA (bound to localhost) to allow sending of email (e.g.,
  password recovery).
- All secrets will be regenerated during installation / firstboot
  (security).
- Webmin modules for configuring Apache2, PHP, MySQL and Postfix.

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH, MySQL: username **root**
-  Adminer: username **adminer**
-  Phorge: username **admin**


.. _Phorge: https://we.phorge.it/
.. _TurnKey Core: https://www.turnkeylinux.org/core
.. _Adminer: https://www.adminer.org/
