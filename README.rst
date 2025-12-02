Observium - Network Management and Monitoring
=============================================

`Phorge`_ is repository system, which succeeds Phabricator.

This appliance includes all the standard features in `TurnKey Core`_,
and on top of that:

- Observium configurations:

    - Installed from upstream source code to /opt/phorge
    - Includes all recommended packages including libvirt for virtual
      machine monitoring.

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
