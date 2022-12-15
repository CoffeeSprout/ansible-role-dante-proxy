coffeesprout.dante-proxy
=========

Installs and configures that Dante Socks proxy, to make your connections go from A to B via C.
Nothing really special


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

#Setup Dante to pass traffic from any to any if you login as dante / inferno. Note: not all browsers support this *glares at Chrome*
    - hosts: servers
      roles:
      - role: cofffeesprout.dante-proxy
        dante_socksmethod: username 
        dante_proxy_users:
        - name: dante
          password: inferno

#Setup Dante to pass traffic from internal network without a login:

    - hosts: servers
      roles:
      - role: cofffeesprout.dante-proxy

License
-------

BSD

Author Information
------------------

Just reach out via Github
