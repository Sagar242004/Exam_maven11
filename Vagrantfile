Vagrant.configure("2") do |config|

  # Manager VM
  config.vm.define "manager-vm" do |manager|
    manager.vm.hostname = "manager-vm"
    manager.vm.network "private_network", ip: "192.168.56.10"

    manager.vm.provider "virtualbox" do |vb|
      vb.memory = 2048
      vb.cpus = 2
    end
  end

  # Worker VM
  config.vm.define "worker1-vm" do |worker|
    worker.vm.hostname = "worker1-vm"
    worker.vm.network "private_network", ip: "192.168.56.11"

    worker.vm.provider "virtualbox" do |vb|
      vb.memory = 1024
      vb.cpus = 1
    end
  end

end
