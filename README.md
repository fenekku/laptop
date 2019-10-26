# The Setup

The Setup is a repo containing scripts to set up a Mac, Ubuntu or Windows
laptop or desktop for development and usage.

It can be run multiple times on the same machine safely.
It installs, upgrades, or skips packages
based on what is already installed on the machine.

## ubuntu

Support for:

* Bionic Beaver (18.04)

Download and execute the script:

	wget --quiet https://raw.github.com/fenekku/the_setup/master/ubuntu --output-document=- | bash

## windows

Support for:

* Windows 10

Download and execute the script (from PowerShell):

	Set-ExecutionPolicy RemoteSigned
	. { iwr -useb https://boxstarter.org/bootstrapper.ps1 } | iex; get-boxstarter -Force
	Install-BoxstarterPackage -PackageName https://raw.githubusercontent.com/fenekku/the_setup/master/windows.txt

After that, install Ubuntu Bash on Windows via the Microsoft Store (search for Ubuntu).
Create a link from Ubuntu environment to your Windows `dev/` directory.

Download and execute the ubuntu_on_windows script:

	wget --quiet https://raw.github.com/fenekku/the_setup/master/ubuntu_on_windows --output-document=- | bash
