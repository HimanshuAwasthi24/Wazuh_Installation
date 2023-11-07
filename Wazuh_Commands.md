# How To Install Wazuh Server on Ubuntu 20.04|18.04
# Setup Pre-requisites
* The minimum hardware requirements are as below: *
1. 4 GB of RAM
2. 2 CPU cores

# Install the packages below needed for the running of Wazuh Manager.

# sudo apt update
 sudo apt install vim curl apt-transport-https unzip wget libcap2-bin software-properties-common lsb-release gnupg2

# Automated install of Wazuh Server on Ubuntu 20.04|18.04 using script

 curl -sO https://packages.wazuh.com/4.3/wazuh-install.sh
 sudo bash ./wazuh-install.sh -a

# save password and username and access the dashboard using your ip

# install Wazuh agent on another server to get log and matrices on wazuh manager

 wget https://packages.wazuh.com/4.x/apt/pool/main/w/wazuh-agent/wazuh-agent_4.6.0-1_amd64.deb && sudo WAZUH_MANAGER='IP or Domain' WAZUH_AGENT_GROUP='name' WAZUH_AGENT_NAME='name' dpkg -i ./wazuh-agent_4.6.0-1_amd64.deb

sudo systemctl daemon-reload

sudo systemctl enable wazuh-agent

sudo systemctl start wazuh-agent




