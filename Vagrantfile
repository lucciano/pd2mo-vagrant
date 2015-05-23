Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.boot_timeout = 120

  config.vm.provider "virtualbox" do |vb|
     vb.gui = true
     vb.memory = "4096"
  end
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
