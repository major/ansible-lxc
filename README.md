## Try out LXC on Fedora 21 with Ansible

This simple [Ansible](http://www.ansible.com/home) playbook will set up [LXC](https://linuxcontainers.org/) on a [Fedora 21](https://getfedora.org/) server.  To be more specific, here's what it does:

1. Installs libvirt and LXC packages
2. Configures services to start at boot
3. Creates a basic Fedora 21 container
4. Registers the container with libvirt
5. Configures the container with a root password ("fedora") and DHCP
6. Starts the container

Once everything is ready, you'll get the container's IP address printed in the console.  It's also compeletely safe to re-run the playbook over and over again if needed.

Let me know what you think.  As always, pull requests are welcome.

*--Major*