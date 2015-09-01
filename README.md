# Basic host setup

Ansible Role for basic setup and configuration of a host machine for the intended purpose.

.. code-block:: yaml

    - name: Basic host setup
      hosts: "{{ host_group|default('hosts') }}"
      max_fail_percentage: 20
      user: root
      roles:
        - { role: "basic-host-setup", tags: [ "basic-host-setup" ] }

Authors and License
-------

Written by:
* George Li | [e-Mail](GeorgeL1357@gmail.com) | [GitHub](https://github.com/GeorgeL1)

Licensed under the Apache License, Version 2.0 (the "License");

Copyright 2015, George Li from [Yongxin Solutions](www.yongxin.info)
