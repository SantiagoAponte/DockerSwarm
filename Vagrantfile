Vagrant.configure("2") do |config|
  config.vm.define :master do |master|
    master.vm.box = "bento/ubuntu-18.04"
    master.vm.network :private_network, ip: "10.0.0.50"
    master.vm.hostname = "master"
  end
  config.vm.define :worker1 do |worker1|
    worker1.vm.box = "bento/ubuntu-18.04"
    worker1.vm.network :private_network, ip: "10.0.0.100"
    worker1.vm.hostname = "worker1"
  end
  config.vm.define :worker2 do |worker2|
    worker2.vm.box = "bento/ubuntu-18.04"
    worker2.vm.network :private_network, ip: "10.0.0.101"
    worker2.vm.hostname = "worker2"
  end
  config.vm.synced_folder ".", "./vagrant", disabled:true
end
