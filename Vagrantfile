PROJECT_NAME = "LearningDocker"
API_VERSION  = "2"

Vagrant.configure(API_VERSION) do |config|
    config.vm.define PROJECT_NAME, primary: true do |config|
        config.vm.provider :virtualbox do |vb|
            vb.name = PROJECT_NAME
            vb.customize [ "guestproperty", "set", :id, "/VirtualBox/GuestAdd/VBoxService/--timesync-set-threshold", 1000 ]
        end

        config.vm.box = "bento/centos-7.2"
        config.ssh.insert_key = false
        config.vm.provision "docker"
    end
end
