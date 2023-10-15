# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|
  
   # Configuração da primeira máquina virtual
   config.vm.define "maquina1" do |maquina1|
    maquina1.vm.box = "ubuntu/trusty64" # Escolha a imagem Ubuntu ou outra de sua preferência
    maquina1.vm.network "private_network", type: "dhcp"

   # Configuração para executar um script shell durante o provisionamento
  config.vm.provision "shell", path: "instala1.sh"
  end

  # Configuração da segunda máquina virtual
  config.vm.define "maquina2" do |maquina2|
    maquina2.vm.box = "centos/7" # Escolha a imagem CentOS ou outra de sua preferência
    maquina2.vm.network "private_network", type: "dhcp"

  # Configuração para executar um script shell durante o provisionamento
  config.vm.provision "shell", path: "instala2.sh"
  end

end


