# Ethereum Hackbox

Vagrant box with Ubuntu and 1337 Ethereum hacking tools.

## Base image

Uses the [gingeleski/ubuntu18_python](https://app.vagrantup.com/gingeleski/boxes/ubuntu18_python) image:

- Ubuntu 18.04
- Python 3
- Git

## Tools

- Mythril OSS
- Manticore

## Known issues

If you get a crash on `vagrant up` like...

- `"vboxsf" is not available`
    - Then you should `vagrant destroy` that box because it'll be incomplete
    - Now run `vagrant plugin install vagrant-vbguest`
    - *Credit to [geerlingguy](https://github.com/geerlingguy) from [this issue](https://github.com/geerlingguy/packer-centos-7/issues/18)!*

## Contributing

Feel free to contribute issues, suggestions, pull requests, you name it.
