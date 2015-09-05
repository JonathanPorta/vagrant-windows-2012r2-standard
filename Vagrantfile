Vagrant.configure("2") do |c|
  c.berkshelf.enabled = false if Vagrant.has_plugin?("vagrant-berkshelf")
  c.vm.box = "jonathanporta/windows-2012r2-standard"
  c.vm.communicator = 'winrm'
  c.winrm.username='vagrant'
  c.winrm.password='vagrant'
  c.vm.provision 'shell', inline: 'ls'
  c.vm.provider :virtualbox do |p|
  end
end
