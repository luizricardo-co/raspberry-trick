install docker on raspbian for raspberry 3b+ and 4

1. Install Docker
curl -sSL https://get.docker.com | sh

2. Add permission to Pi User to run Docker Commands
sudo usermod -aG docker pi

3. Reboot 
sudo reboot 

4. Test Docker installation
docker run hello-world

5. Install proper dependencies
sudo apt-get install -y libffi-dev libssl-dev

sudo apt-get install -y python3 python3-pip

sudo apt-get remove python-configparser

6. Install Docker Compose
sudo pip3 -v install docker-compose