# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "precise64"
  config.vm.box_url = "http://files.vagrantup.com/precise64.box"
  config.vm.network "public_network"
  config.vm.provision :shell, :path => "bootstrap.sh"
  config.vm.synced_folder "../emenu_server/", "/home/vagrant/emenu_server/"
  #config.vm.synced_folder "../emenu_server/target/CloudMenuServer/", "/var/lib/tomcat7/webapps/ROOT/"
end
