Vagrant.configure("2") do |config|
  config.vm.box = "chef/centos-6.5"
  config.vm.provision :shell, path: "bootstrap.sh"
  config.vm.network "forwarded_port", guest: 3000, host: 4567, auto_correct: true
  config.vm.network "forwarded_port", guest: 80, host: 8888
  config.vm.synced_folder "~/Framgia_Projects/Temona", "/home/vagrant/Framgia_Projects/Temona"
end
