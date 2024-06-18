# Developer Environment Setup on Ubuntu 22.04

## Step 1: Install Ubuntu 22.04
1. **Download Ubuntu 22.04**: 
   - Downloaded from the [official Ubuntu download page](https://releases.ubuntu.com/22.04/).
   
2. **Create a Bootable USB Drive**: 
   - Used Rufus (Windows) to create a bootable USB drive.

   - On Linux, the `dd` command can be used:
     bash

     sudo dd if=~/Downloads/ubuntu-22.04-desktop-amd64.iso of=/dev/sdX bs=4M status=progress && sync
     
     Replace `~/Downloads/ubuntu-22.04-desktop-amd64.iso` with the path to the downloaded ISO and `/dev/sdX` with the correct USB drive identifier.

3. **Install Ubuntu**:

   - Booted from the USB drive and followed the installation instructions.

**4 Install Visual Studio Code**

. **Download Visual Studio Code**:

   - Downloaded the `.deb` package from the Visual Studio Code from the the gui ubuntu sw



**4 Set Up Version Control System**
sudo apt update

sudo apt install git

git config --global user.name "urbanus-dev"

git config --global user.email "urbanuswambua2019@gmil.com"

**5 Create a GitHub Account**
Created an account at GitHub.

**Initialize a Git Repository:**

mkdir myProject

cd myProject

git init

touch README.md

git add README.md

git commit -m "Initial commit"


**6 Install Necessary Programming Languages and Runtimes**

sudo apt update

sudo apt install python3 python3-pip

pip3 --version

**7 Configure a Database (MySQL)**

sudo apt update

sudo apt install mysql-server

sudo mysql_secure_installation

**Start MySQL Service**

sudo systemctl start mysql

**8 Set Up Development Environments and Virtualization (Optional)**
sudo apt update

sudo apt install apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt update

sudo apt install docker-ce


sudo systemctl status docker

docker --version



**Challenges Faced**
Encountered issues with MySQL installation where mysql_secure_installation failed to run properly.

Solution: Reconfigured MySQL and ensured all steps were followed correctly.

**Strategies Employed**
Followed the official documentation for each tool and sought help from online forums and community support when issues were encountered.

Used step-by-step guides and verified each step to ensure proper installation and configuration.