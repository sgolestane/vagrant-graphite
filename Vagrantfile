VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.box = "precise64"
  config.vm.box_url = "http://files.vagrantup.com/precise64.box"

  config.vm.network 'forwarded_port', guest: 80, host: 2000
  config.vm.network 'forwarded_port', guest: 8126, host: 8126

  config.vm.provision 'chef_solo' do |chef|
    chef.add_recipe 'apt'
    chef.add_recipe 'graphite'
  end

end