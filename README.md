Role Name
=========

Installation of Confluent Platform Open Source on Ubuntu


Requirements
------------

Ubuntu LTS
Ansible 2.4

Role Variables
--------------
Host groups:
 - kafka
 - zookeeper

global vars:

# Platforms version
cp_version: '4.0'

# Scala instalation version
scala_verison: '2.11'

# Kafka configuration directory
kafka_conf_dir: /etc/kafka

# Zookeeper data directory
zookeeper_data_dir: /var/lib/zookeeper

# Kafka data directory
kafka_data_dir: /var/lib/kafka

# Schema Registry configuration directory
schema_conf_dir: /etc/schema-registry

# Kafka Utils directory
kafka_utils_dir: "/etc/kafka_discovery"


Dependencies
------------

No

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ngaloha.ansible-confluent }

License
-------

Apache

Author Information
------------------
Nazar Halokha
