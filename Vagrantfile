Vagrant.configure("2") do |config|
  config.vm.box = "debian-7.5.0-amd64"
  config.vm.box_url = "https://googledrive.com/host/0B83ZToJ3fGtDVC1DeVVzc3lkc0U/debian-7.5.0-amd64_virtualbox.box"

  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--memory", "512"]
    vb.customize ["modifyvm", :id, "--cpus", "2"]
  end

  config.vm.provision :ansible do |ansible|
    ansible.sudo = true
    ansible.host_key_checking = false
    ansible.playbook = "playbook.yml"
    ansible.verbose = "vv"
    #ansible.tags = ""
  end
end
