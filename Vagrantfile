Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.hostname = "Docker-Server"
  config.vm.network "private_network", ip: "192.168.10.11" 
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "docker_provision.yml"
  end
end
