Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "forwarded_port", guest: 80, host: 8181
  config.vm.network "forwarded_port", guest: 443, host: 8443
end
