VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "precise64"
  config.vm.network :private_network, ip: "33.33.33.10"
  config.vm.synced_folder ".", "/vagrant", :nfs => true
end
