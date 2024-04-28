Ubuntu 20.04
sudo apt-get update
sudo apt-get install apt-transport-https ca-certificates wget

Import the PGP key used to sign our packages:
wget -qO- https://dl.packager.io/srv/opf/openproject/key | sudo apt-key add -

Add the OpenProject package source:
sudo wget -O /etc/apt/sources.list.d/openproject.list https://dl.packager.io/srv/opf/openproject/stable/14/installer/ubuntu/20.04.repo

Download the OpenProject package:
sudo apt-get update
sudo apt-get install openproject
