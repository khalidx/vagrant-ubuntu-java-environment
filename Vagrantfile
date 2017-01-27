# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"

  config.vm.network "forwarded_port", guest: 8080, host: 8080

  config.vm.synced_folder ".", "/project"

  config.vm.provision "shell", inline: <<-SHELL

    echo "Update package lists..."
    sudo apt-get update

    echo "Install Java 8"
    sudo apt-get install -y software-properties-common python-software-properties
    echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | sudo /usr/bin/debconf-set-selections
    sudo add-apt-repository ppa:webupd8team/java -y
    sudo apt-get update
    sudo apt-get install oracle-java8-installer

    echo "Set environment variables for Java 8"
    sudo apt-get install -y oracle-java8-set-default

    echo "Install Maven"
    sudo apt-get install -y maven

  SHELL

end
