# UCLALib Ansible Role: Handle

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

