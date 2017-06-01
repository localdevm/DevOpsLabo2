
Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/precise64"
  config.vm.hostname="maarten.be"
  config.vm.network "private_network", ip: "172.16.240.81"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.provision "shell", path: "web.sh"
  config.ssh.insert_key = false
end
