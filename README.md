[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vbnbTt5m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15292006&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment
#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. **Select Your Operating System (OS):**
   Choose an operating system that best suits your preferences and project requirements.

   Download Ubuntu 22.04: Go to the official Ubuntu download page and download the ISO file.https://releases.ubuntu.com/22.04/

   ![alt text](image.png)
   Create a Bootable USB Drive: Use tools like Rufus (Windows) or dd (Linux) to create a bootable USB drive.
   ![alt text](image-1.png)
   ![alt text](image-2.png)

   Install Ubuntu: Boot from the USB drive and follow the installation instructions.
   ![alt text](image-3.png)
   ![alt text](image-4.png)
   ![alt text](image-5.png)
   ![alt text](image-6.png)
   ![alt text](image-7.png)

   installation 
   ![alt text](image-8.png)
   ![alt text](image-9.png)
   ![alt text](image-10.png)
   ![alt text](image-11.png)
   ![alt text](image-12.png)
   ![alt text](image-13.png)
   ![alt text](image-14.png)


**2. Install a Text Editor or Integrated Development Environment (IDE):**

 Install Visual Studio Code.I installed it using the GUI
visit this

![alt text](image-15.png)
![alt text](image-16.png)
![alt text](image-17.png)
![alt text](image-18.png)
![alt text](image-19.png)

**3. Set Up Version Control System:**

   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit.

   installation

   sudo apt update

   sudo apt install git

   ![alt text](image-20.png)

   Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit.
      
git config --global user.name "urbanus-dev"

git config --global user.email "urbanuswambua2019@gmail.com"

      mkdir myProject

      cd myProject

      git init

      touch README.md

      git add README.md

      git commit -m "Initial commit"

      https://github.com/urbanus-dev/myProject

**4. Install Necessary Programming Languages and Runtimes:**

  Instal Python 

  sudo apt update

  sudo apt install python3 python3-pip

 ![alt text](image-22.png)


**5. Install Package Managers:**

   If applicable, install package managers like pip (Python).

   pip: Already installed with Python in the previous step

   ![alt text](image-23.png)


**6. Configure a Database (MySQL):**

sudo apt update

sudo apt install mysql-server

sudo systemctl start mysql

sudo mysql -u root -p

  ![alt text](image-24.png)
  ![alt text](image-25.png)

**7. Set Up Development Environments and Virtualization (Optional):**
 

**8. Explore Extensions and Plugins:**

   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.

sudo apt update

sudo apt install apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg

echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt update

sudo apt install docker-ce

sudo systemctl status docker

![alt text](image-26.png)

docker --version

![alt text](image-27.png)

Open VS Code

Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window or by pressing Ctrl+Shift+X.
Search and install the following extensions:

Python

GitLens

Docker