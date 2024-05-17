Jenkins Installation
####################

Steps to install Jenkins
----------------------
sudo wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt update
sudo apt install jenkins
sudo sysemctl start jenkins
sudo systemctl status jenkins
sudo systemctl restart jenkins
sudo systemctl enable jenkins ( Bootup start)

How to give sudo permissions for jenkins user in Ubuntu machine?

Open a file using vi editor or gedit in ubuntu
1) sudo vi /etc/sudoers or sudo gedit /etc/sudoers
2) add below line in sudoers file
jenkins ALL=(ALL) NOPASSWD: ALL
3)sudo systemctl restart jenkins

########
