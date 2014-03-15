# Vagrant

[Vagrant](http://www.vagrantup.com/) provides an easy way to create and configure portable development enviroments.
We will use it to create an Ubunutu VM and install Docker.

In order to use the Docker provisioner you'll need a Vagrant box that is ready for Docker.

```
config.vm.box = "raring64"
config.vm.box_url = "http://cloud-images.ubuntu.com/vagrant/raring/current/raring-server-cloudimg-amd64-vagrant-disk1.box"
```

[download Vagrant](http://www.vagrantup.com/downloads.html)

Talk about synced folders and ownership by the www-data user
