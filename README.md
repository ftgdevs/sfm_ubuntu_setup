
# create new ubuntu virtual machine

# logon and ensure that git is installed
sudo apt-get -y install git-core

# clone this repo to your user directory
git clone git@github.com:bhedana/sfm_ubuntu_setup.git sfmdev

# move into the directory
cd sfm_dev

# execute script to load development dependencies
./setup_dependencies

# execute script to load development environment
./setup_environment

# execute script to checkout and configure application
./setup_sfm