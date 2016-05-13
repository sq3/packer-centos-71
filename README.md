# Packer CentOS 7.1 template

This template generates a CentOS 7.1 vagrant box, VirtualBox VM or
VMWare VM.

## Overview

64-bit
40 GB disk
512 MB memory
OpenSSH for vagrant is also installed

## Usage

# VirtualBox / Vagrant Provider

Assuming that you already have Packer, VirtualBox, and Vagrant installed,
you should be good to clone this repo and go:

	$ git clone https://github.com/sq3/packer-centos-71.git
	$ cd packer-centos-71/
	$ packer build -only=virtualbox-iso template.json

Then you can import the generated box into Vagrant:

	$ vagrant box add arch centos-71-virtualbox.box
	$ vagrant up

The vagrantfil uses VirtuaBos linked clones (copy-on-write)

	v.linked_clone = true
