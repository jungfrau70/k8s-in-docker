# k8s-in-docker

################################################################################################
# 1. Install Utils
################################################################################################

sudo apt install -y net-tools git wget curl
ifconfig


################################################################################################
# 2. Download git repo
################################################################################################

# switch to root
sudo passwd
su -

# clone git repo
cd 
git clone https://github.com/jungfrau70/k8s-in-docker.git


################################################################################################
# 3. Install OpenSSH server
################################################################################################
cd
cd k8s-in-docker/kind
bash config/install-openssh.sh

################################################################################################
# 4. Check ip
################################################################################################

ifconfig | grep inet

################################################################################################
# 5. Enable Remoto-SSH in vscode
################################################################################################

C:\Users\inhwa\.ssh\config
Host deploy-server
  HostName 192.168.171.129
  User root
  # IdentityFile C:\Users\inhwa\.ssh\cloud9.pem


################################################################################################
# 6. Connect to VM via Remote-SSH
################################################################################################
