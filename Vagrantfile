### Vagrant file for bash Script###

Vagrant.configure("2") do |config|

  config.vm.define "scriptbox" do |scriptbox|
    scriptbox.vm.box = "eurolinux-vagrant/centos-stream-9"
	scriptbox.vm.network "private_network", ip: "192.168.10.12"
        scriptbox.vm.hostname = "scriptbox"
	scriptbox.vm.provider "virtualbox" do |vb|
     vb.memory = "1024"
   end
  end

  config.vm.define "web01" do |web01|
    web01.vm.box = "eurolinux-vagrant/centos-stream-9"
	web01.vm.network "private_network", ip: "192.168.10.13"
        web01.vm.hostname = "web01"
  end
  
  config.vm.define "web02" do |web02|
    web02.vm.box = "eurolinux-vagrant/centos-stream-9"
	web02.vm.network "private_network", ip: "192.168.10.14"
        web02.vm.hostname = "web02"
  end

   config.vm.define "web03" do |web03|
    web03.vm.box = "ubuntu/bionic64"
        web03.vm.network "private_network", ip: "192.168.10.15"
        web03.vm.hostname = "web03"
  end
end
