# vagrant-ubuntu-java-environment
A simple Vagrant configuration file to setup a development environment for Java on Ubuntu.
This configuration also installs Maven.

## Using the Vagrantfile to spin up an evironment
1. Make sure you have Vagrant installed (you can grab the installation for your OS at https://www.vagrantup.com/)
2. Clone this repository locally (or alternatively, just download the Vagrantfile)
3. Go into the directory that has the Vagrantfile you just downloaded and run `vagrant up`
4. That's it! You now have a Java development environment!
5. Now, you can easily:
  1. SSH into the environment by running `vagrant ssh`
  2. stop your environment with `vagrant halt`
  3. destroy your environment with `vagrant destroy`

## Support
Please contact kzoabi@outlook.com for questions or suggestions.
You may also make changes yourself and open a pull request to have your changes merged.
