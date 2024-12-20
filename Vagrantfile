Vagrant.configure("2") do |config|
  # First machine configuration
  config.vm.define "machine1" do |machine|
    machine.vm.box = "ubuntu/bionic64"
    machine.vm.provider "virtualbox" do |vb|
      vb.memory = "512"  # Set memory to 512MB
      vb.cpus = 1        # Set CPUs to 1
    end
    # Assign static IP to machine1
    machine.vm.network "private_network", ip: "192.168.56.15"
  end

  # Second machine configuration
  config.vm.define "machine2" do |machine|
    machine.vm.box = "ubuntu/bionic64"
    machine.vm.provider "virtualbox" do |vb|
      vb.memory = "512"  # Set memory to 512MB
      vb.cpus = 1        # Set CPUs to 1
    end
    # Assign static IP to machine2
    machine.vm.network "private_network", ip: "192.168.56.16"
  end
end

