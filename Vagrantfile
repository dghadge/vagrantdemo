# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.hostname = "hubot-dev"
  config.vm.provision "shell", path: "provision.sh"
  config.vm.synced_folder ".", "/vagrant", type: "rsync", rsync_exclude: [".git/", "myhubot/node_modules"]
end
