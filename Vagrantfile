Vagrant.configure("2") do |config|
    config.vm.box = "generic/ubuntu2004"
  
    config.vm.network "forwarded_port", guest: 3000, host: 3000
  
    config.vm.provision "ansible" do |ansible|
      ansible.playbook = "ansible/playbook.yml"
    end
  end