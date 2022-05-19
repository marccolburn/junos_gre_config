GRE Configuration
=========

Configure GRE Tunnels for Junos.

Requirements
------------


Role Variables
--------------
gre_tunnels: List of Dictionaries containing GRE tunnel src, dest, and address.
* interface: Name of tunnel interface, string
* unit: unit of interface, int
* src: source address of tunnel, string
* dest: destination address of tunnel, string
* address: IP address of tunnel, string

gre_settings: Dictionary containing settings for GRE tunnels
* tun_bandwidth: Sets bandwidth allocated to tunnel services on platform, string


Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: junos_isis_config }

License
-------

BSD

Author Information
------------------

Marc Colburn Juniper
