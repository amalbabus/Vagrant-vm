# -*- mode: ruby -*-

Vagrant.configure("2") do |config|


  config.vm.box = "ubuntu/xenial64"



  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
   config.vm.network "private_network", ip: "192.168.56.10"


  # sync folder  
  #  config.vm.synced_folder "", "/vagrant_data", SharedFoldersEnableSymlinksCreate: false

  # Provider-specific configuration so you can fine-tune various
  # backing providers for Vagrant. These expose provider-specific options.
  # Example for VirtualBox:
  #
  config.vm.provider "virtualbox" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
  #   vb.gui = true
  #
    # Customize the amount of memory on the VM:
    vb.memory = "4096"
    vb.cpus = "2"
  end
  config.vm.provision "shell", path: "installer.sh" 
  
  

end
