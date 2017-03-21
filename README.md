# UCLALib Ansible Role: Handle [![Build Status](https://travis-ci.org/UCLALibrary/uclalib_role_handle.svg?branch=master)](https://travis-ci.org/UCLALibrary/uclalib_role_handle)

Installs a Handle service on RHEL servers. The Handle service utilizes the [DSpace Remote Handle Resolver](https://github.com/DSpace/Remote-Handle-Resolver) plugin with the stock Handle service from CNRI. This setup is [documented on the DuraSpace wiki](https://wiki.duraspace.org/display/~pbecker/MultiRemoteDSpaceRepositoryHandlePlugin).

## What do you get when this role is done?

This role installs a stock Handle service (version number is specified via a variable, see below). The [DSpace Remote Handle Resolver](https://github.com/DSpace/Remote-Handle-Resolver) plugin is installed and configured. It is left up to you to run the final configuration steps (see the README.txt file in ```/usr/local/handle```) and to forward the sitebndl.zip file produced by the installation script to CNRI.

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
