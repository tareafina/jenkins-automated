Vagrant.configure("2") do |config|
  config.vm.define "master" do |master|
    master.vm.box = "bento/ubuntu-18.04"
    master.vm.hostname = "jenkinsMaster"
    master.vm.network :private_network, ip: "192.168.56.10"
    end
  
  config.vm.define "slave" do |slave|
    slave.vm.box = "bento/ubuntu-18.04"
    slave.vm.hostname = "jenkinsSlave"
    slave.vm.network :private_network, ip: "192.168.56.11"
    end
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "./ansible/site.yml"
    ansible.groups = {
      "jenkins" => ["192.168.56.10", "192.168.56.11"]
    }
  end

end
