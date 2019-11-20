Automate_elasticsearch
=========

This role installs and configures elasticsearch. This role includes the following:

  * https://www.elastic.co/guide/en/elasticsearch/reference/7.3/rpm.html#rpm-enable-indices[Enabled system indices]

   * Removed the --quiet option so you can get a status https://www.elastic.co/guide/en/elasticsearch/reference/7.3/rpm.html#rpm-running-systemd


Requirements
------------

A

Role Variables
--------------



Dependencies
------------



Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: elasticsearch
      roles:
         - automate_elasticsearch

License
-------

GPLv3

Author Information
------------------


