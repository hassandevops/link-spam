Vagrant.configure("2") do |config|
  config.vm.network "public_network", bridge: "eno1"
  config.vm.define "web" do |web|
  web.vm.box = "ubuntu/trusty64"
  web.vm.hostname = 'web'
end

 config.vm.define "db" do |db|
 db.vm.box = "aerospike/centos-6.5"
 db.vm.hostname = 'db' 
end
 config.vm.provider "virtualbox" do |vb|
 vb.memory = "2048"
end
end
