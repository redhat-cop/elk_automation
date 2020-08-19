Automate_elasticsearch
=========

This role installs and configures elasticsearch. This role includes the following:

  * https://www.elastic.co/guide/en/elasticsearch/reference/7.3/rpm.html#rpm-enable-indices[Enabled system indices]

   * Removed the --quiet option so you can get a status https://www.elastic.co/guide/en/elasticsearch/reference/7.3/rpm.html#rpm-running-systemd

This role has the option to either create the yum repository using a template or using the yum repository module.

Requirements
------------



Role Variables
--------------

elasticsearch_install: "True"
elasticsearch_configure: "True"
elasticsearch_repo: "True"
yum_repo: "False"
elasticsearch_service_dir: "/usr/lib/systemd/system/elasticsearch.service"
elasticsearch_service_file: "elasticsearch.service"
elasticsearch_config_dest: "/etc/elasticsearch/elasticsearch.yml"
elasticsearch_config_template: "elasticsearch.j2.yml"
elasticsearch_yum_repo_template_dest: "/etc/yum.repos.d/elasticsearch.repo"
elasticsearch_yum_repo_template_file: "elasticsearch.j2.repo"
elasticsearch_yum_name: "elasticsearch"
elasticsearch_yum_repo_name: "Elasticsearch repository for 7.x packages"
elasticsearch_data_dir: "/var/lib/elasticsearch"
elasticsearch_data_logs: "/var/log/elasticsearch"
elasticsearch_cluster_name: "mycluster"
elasticsearc_node_attribute: "myrack"

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

jlozadad@redhat.com

