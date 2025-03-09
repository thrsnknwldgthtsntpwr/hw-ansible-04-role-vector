Vector-role
=========

This role allows you to install Vector on Debian-based distros

Role Variables
--------------

| vars | Description | Value | Location |
|------|------------|---|---|
| vector_version | Vector version to install | "0.42.0" | defaults/main.yml |
| vector_rpm_version | Vector rmp version to use for installation | "0.42.0-1" | defaults/main.yml |
| vector_clickhouse_ip | An instance for Clickhouse to work with Vector | for ex., "localhost" | defaults/main.yml |
| clickhouse_db_name | Clickhouse DB name for logs | "logs"  | defaults/main.yml |
| clickhouse_table_name | Clickhouse table name to write down logs | "data_logs" | defaults/main.yml |
| vector_config | Vector configuration settings | wwritten down below, may be changed | default/main.yml |
| vector_url | URL for Vector packages | "https://yum.vector.dev/stable/vector-0/x86_64/vector-{{ vector_rpm_version }}.x86_64.rpm" | vars/main.yml |
| vector_config_dir | Vector config file location | "/etc/vector" | vars/main.yml |


License
-------

MIT

Author Information
------------------

Roman Nikiforov
