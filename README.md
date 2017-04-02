VPN-Router
=========

Sets up a simple VPN Gateway based on OpenVPN and IPTables

Requirements
------------

Debian Jessie is so far what's been tested.

Role Variables
--------------

* enable_reboot - [boolean] Sets whether to reboot on finishing or not(Default:true)
* ovpn_cert - [string] The ovpn file contents to start OpenVPN with. Make sure the 'redirect-gateway def1' is in the config.
* ovpn_dev - [string] The device to use for the VPN (Default:tun0)

Dependencies
------------

[None]

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      become: yes
      become_method: sudo
      roles:
         - { role: ansible-role-vpn-router }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
