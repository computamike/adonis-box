Vagrant.configure("2") do |config|
  config.vm.box = "apcovernight/adonis-box"
  config.vm.box_version = "0.0.2"
  config.vm.network "private_network", ip: "192.168.33.10"
  config.vm.network "forwarded_port", guest: 3306, host: 3306
  config.vm.hostname = "adonis-box"
  config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]
end
