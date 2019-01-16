# VMs

Vagrant VMs for various testing of YouCompleteMe and other stuff. If it is useful, go ahead and use it. Otherwise, get off my lawn.

# Usage

* Install [Vagrant](http://vagrantup.com)
* Install [VirtualBox](https://www.virtualbox.org)
* `cd` to the directory containing the VM you want to test (e.g. Ubuntu 18.04 LTS)
* `vagrant up`
* Wait a bit
* `vagrant ssh`

From here you should now be in a position to run `vim` and get [my Vim configuration][pm-vim] with YCM installed and working.  Lucky you.

# Running ycmd tests

* `vagrant ssh`
* `cd $HOME/.vim/bundle/YouCompleteMe-Clean/third_party/ycmd`
* `./run_tests.py --skip-build` (for example, see `TESTS.md` for more info)

# Contributing

PRs always welcome, to:

* Fix bugs
* Add providers
* Add machines, assuming they work completely cleanly from `vagrant up`
