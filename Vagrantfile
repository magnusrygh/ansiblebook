VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.ssh.insert_key = false

  config.vm.define "ansvagrant1" do |vagrant1|
    vagrant1.vm.box = "ubuntu/trusty64"
    vagrant1.vm.network "forwarded_port", guest: 80, host: 8181
    vagrant1.vm.network "forwarded_port", guest: 443, host: 8443
    vagrant1.vm.network "forwarded_port", guest: 8000, host: 8000
  end
  config.vm.define "ansvagrant2" do |vagrant2|
    vagrant2.vm.box = "ubuntu/trusty64"
    vagrant2.vm.network "forwarded_port", guest: 80, host: 8182
    vagrant2.vm.network "forwarded_port", guest: 443, host: 8444
  end
  config.vm.define "ansvagrant3" do |vagrant3|
    vagrant3.vm.box = "ubuntu/trusty64"
    vagrant3.vm.network "forwarded_port", guest: 80, host: 8183
    vagrant3.vm.network "forwarded_port", guest: 443, host: 8445
  end
end
