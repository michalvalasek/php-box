php-box
=======

Vagrant box for PHP development (LAMP)

Tested with Vagrant `1.3.5` and VirtualBox `4.2.16`.

###Setup
1. Install VirtualBox and Vagrant.
2. Clone this repository: `git clone git@github.com:michalvalasek/php-box.git && cd php-box`
3. Start the VM: `vagrant up`
4. After first start: `vagrant provision`
5. Add to your hosts file: `192.168.111.111 adminer.phpbox`

###Adding vhosts
1. Edit file `puppet/hieradata/common.yaml` and add the new vhost under section: `vagrantfile-local`/`apache`/`vhosts`.
2. Add the new vhost to your hosts file: `192.168.111.111 your-new-vhost.phpbox`
