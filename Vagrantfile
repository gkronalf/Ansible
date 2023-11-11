Vagrant.configure("2") do |nginx|
 nginx.vm.box = "ubuntu/focal64"

 nginx.vm.provider "virtualbox" do |i|
  i.name = "vm_nginx"
  i.memory = "2048"
  i.cpus = 2
 end
 nginx.vm.network "forwarded_port", host: 8000, guest: 80
end