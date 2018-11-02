Vagrant.configure("2") do |config|

  config.vm.box = "bento/ubuntu-16.04"

  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
  end

  config.vm.provider "virtualbox" do |v|
    v.customize ["modifyvm", :id, "--cpuexecutioncap", "100"]
  end
  
  config.vm.network "private_network", ip: "10.10.10.20"
  
  config.vm.provision "ansible_local" do |a|
    a.playbook = "setup.yml"
  end
end
