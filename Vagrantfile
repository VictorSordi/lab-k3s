Vagrant.configure("2") do |config|
    config.vm.box = "bento/ubuntu-22.04"
    config.vm.hostname = 'manager'
    config.vm.network "private_network", ip: "192.168.56.8"
    config.vm.provider 'virtualbox' do |v|
        v.memory = 4096
    end
end