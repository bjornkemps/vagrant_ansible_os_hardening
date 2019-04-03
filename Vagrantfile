Vagrant.configure("2") do |config|
  config.vm.box = "geerlingguy/centos7"

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.customize ["modifyvm", :id, "--memory", "3192"] # Needs minimally 3192
  end

  # Prov
  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "book.yml"
    ansible.verbose = true
    # ansible.extra_vars = 'ansible-vars-override.yml' # using book.yaml's vars variable for this
  end
end
