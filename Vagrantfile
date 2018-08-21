$INSTALL_RUSTUP = "curl https://sh.rustup.rs -sSf | sh -s -- -y"

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"

  config.vm.provision "Install rustup",
                      type: "shell",
                      inline: $INSTALL_RUSTUP,
                      privileged: false
end
