
# create new ubuntu virtual machine

# logon and ensure that git is installed
sudo apt-get -y install git-core

# clone this repo to your user directory
git clone https://github.com/bhedana/sfm_ubuntu_setup.git sfmdev

# move into the directory
cd sfm_dev

# execute script to load development dependencies
./setup_dependencies

# execute script to load development environment
./setup_environment

NOTE: The install script for bash-it will also prompt you asking if you use Jekyll. 
This is to set up the .jekyllconfig file, which stores info necessary to use the Jekyll plugin.

Also it will ask which aliases and plugins you want to activate.. for now answer none..
see https://github.com/revans/bash-it for more info 

# execute script to checkout and configure application
./setup_sfm

open new terminal window or source ~/.bashrc to finalize environment changes