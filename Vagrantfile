# Vagrant.configure("2") do |config|
#     config.vm.box = "generic/ubuntu2004"
  
#     config.vm.network "forwarded_port", guest: 3000, host: 3000
  
#     config.vm.provision "ansible" do |ansible|
#       ansible.playbook = "ansible/playbook.yml"
#     end
#   end


Vagrant.configure("2") do |config|
    # General configuration
    config.vm.box = "generic/ubuntu2004"
#    config.vm.hostname = "kiosk.localdomain"

#    config.vm.network "private_network", ip: "192.168.56.10"
#    config.vm.network :forwarded_port, guest: 22, host: 2522, auto_correct: false, id: "ssh"
      auto_config= false
    config.vm.synced_folder '.', '/vagrant', disabled: true

    config.vm.provision "ansible" do |ansible|
      ansible.playbook = "ansible/playbook.yml"
    end
end