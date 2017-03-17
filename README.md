# UCLALib Ansible Role: Handle [![Build Status](https://travis-ci.org/UCLALibrary/uclalib_role_handle.svg?branch=master)](https://travis-ci.org/UCLALibrary/uclalib_role_handle)

Installs a Handle service on RHEL servers

## Variables

  handle_version - defines the full version of handle to use (e.g. 8.1)

  Example:
  ```
  ---
  - name: uclalib_handle_param.yml
    sudo: true
    hosts: test

    roles:
      - { role: uclalib_role_java }
  ```
