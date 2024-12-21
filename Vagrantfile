Vagrant.configure("2") do |config|
    ### VM3 ###
    config.vm.define "m03" do |m03|
        m03.vm.box = "ubuntu/jammy64"
        m03.vm.hostname = "m03"
        m03.vm.network "private_network", ip: "192.168.56.15"
        m03.vm.provider "virtualbox" do |vb|
            vb.gui = true
            vb.memory = "600"
        end
    end

    ### VM4 ###
    config.vm.define "m01" do |m01|
        m01.vm.box = "ubuntu/jammy64"
        m01.vm.hostname = "m01"
        m01.vm.network "private_network", ip: "192.168.56.16"
        m01.vm.provider "virtualbox" do |vb|
            vb.gui = true
            vb.memory = "600"
        end
    end
end
