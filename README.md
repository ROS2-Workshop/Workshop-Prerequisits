# ROS-Workshop prerequisits


1. Visual Studio Code
2. Git and tiling termnial
3. ROS2 Humble


The following commands should install all prerequisits:

## Visual Studio Code

Visual studio will be the default text-editor during the workshop, other IDE's or text-editors can be used BUT no assistance will be provided towards IDE/text-editor related issues.

```bash
sudo apt update -y && sudo apt upgrade -y
sudo apt install software-properties-common apt-transport-https wget -y
wget -O- https://packages.microsoft.com/keys/microsoft.asc | sudo gpg --dearmor | sudo tee /usr/share/keyrings/vscode.gpg
echo deb [arch=amd64 signed-by=/usr/share/keyrings/vscode.gpg] https://packages.microsoft.com/repos/vscode stable main | sudo tee /etc/apt/sources.list.d/vscode.list
sudo apt update
sudo apt install code
```


## Git , terminal & others

Git will be used for cloning demos and the terminal 'terminator' will be used for tiling a terminal rather than having multiple terminals.

```bash
sudo apt install terminator python-is-python3 git wget curl -y
```

## ROS2 Humble 

The following script will install ROS2 Humble Desktop (Full version).

```bash
git clone https://github.com/ROS2-Workshop/ros2_setup_scripts_ubuntu
cd ros2_setup_scripts_ubuntu 
./run.sh
```

