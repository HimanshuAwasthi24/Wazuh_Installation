# How To Install Wazuh Server on Ubuntu 20.04|18.04
# Setup Pre-requisites
* The minimum hardware requirements are as below: *
1. 4 GB of RAM
2. 2 CPU cores

# Install the packages below needed for the running of Wazuh Manager.

## sudo apt update
## sudo apt install vim curl apt-transport-https unzip wget libcap2-bin software-properties-common lsb-release gnupg2

# Automated install of Wazuh Server on Ubuntu 20.04|18.04 using script

## curl -sO https://packages.wazuh.com/4.3/wazuh-install.sh
## sudo bash ./wazuh-install.sh -a

# save password and username and access the dashboard using your ip
