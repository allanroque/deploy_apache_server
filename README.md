deploy_apache_server
=========

This Ansible role automates the installation of the Apache web server, making it ideal for test environments, demonstrations, or development purposes. It focuses on a simple setup to quickly get an Apache server running on Linux systems.

Requirements
------------

No special requirements. Ensure that port 80 (HTTP) is open and available on the target server to allow web traffic.

Role Variables
--------------

This role includes a customizable variable for setting a test message, which can be used to validate the Apache installation and configuration through a simple web page display.

Variable: apache_test_message

Default Message: "Test apache e automation"


Example Playbook
----------------

````
- hosts: servers
  become: True
  roles:
    - deploy_apache_server
````

License
-------

MIT