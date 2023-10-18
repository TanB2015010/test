$sudo apt install openjdk-11-jdk -y
$wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
$sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
$sudo apt update ; sudo apt install jenkins -y

- Launch Jenkins
$sudo usermod -aG docker jenkins
$sudo systemctl restart jenkins.service

# test
