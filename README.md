# puppet-sandbox

This project uses puppet and vagrant to create a Puppet Enterprise dev sandbox environment.

It installs and configures:
* [Puppet Enterprise 2015.3.2 Master](https://puppetlabs.com/puppet/puppet-enterprise).

## Prerequisites
* Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
* Install [Vagrant](http://www.vagrantup.com/downloads.html)
* Install the following Vagrant plugins:
  * `$ vagrant plugin install oscar`
  * `$ vagrant plugin install vagrant-multiprovider-snap`
  * `$ vagrant plugin install vagrant-reload`
  * `$ vagrant plugin install vagrant-hosts`

## Running
1. `vagrant up`
2. `vagrant hosts puppetize | sudo puppet apply`
3. Access the PE console via https://master.inf.puppetlabs.demo (admin/puppetlabs)
