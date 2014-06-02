Installation Instructions

1. Install VirtualBox and add it to your system PATH

2. Install Vagrant

3. Install Vagrant plugins
   $ vagrant plugin install vagrant-berkshelf
   $ vagrant plugin install vagrant-omnibus
   $ vagrant plugin install vagrant-cachier

4. Download Ubuntu 14.04 from the link below: http://opscode-vm-bento.s3.amazonaws.com/vagrant/vmware/opscode_ubuntu-14.04_chef-provisionerless.box 
   And store it in the directory: C:\DevOps\Vagrant\boxes

====
Creating VM

5. Run command:
   $ vagrant init vagrant-hackaton http://opscode-vm-bento.s3.amazonaws.com/vagrant/vmware/opscode_ubuntu-14.04_chef-provisionerless.box

It will create Vagrantfile (configuration for Vagrant)

6. Run command:
   $ vagrant up

Vagrant will start to download image. Interrupt it (CTRL+C)!!! We have already Linux image in our Disk

6. $ vagrant box list 

7. $ vagrant box add vagrant-hackaton C:\DevOps\Vagrant\boxes\opscode_ubuntu-14.04_chef-provisionerless.box
   $ vagrant up
   $ vagrant ssh

You are in :)

8. $ vagrant halt
To stop VM

9. $ vagrant destroy
To delte VM (as it never existed)