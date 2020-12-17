# 7inch screen enable

Enter on config.txt

```sh
sudo nano /boot/config.txt
```

# install docker on raspbian for raspberry 3b+ and 4

Install Docker

```sh
curl -sSL https://get.docker.com | sh
```

Add permission to Pi User to run Docker Commands

```sh
sudo usermod -aG docker pi
```

Reboot

```sh
sudo reboot
```

Test Docker installation

```sh
docker run hello-world
```

Install proper dependencies

```sh
sudo apt-get install -y libffi-dev libssl-dev
sudo apt-get install -y python3 python3-pip
sudo apt-get remove python-configparser
```

Install Docker Compose

```sh
sudo pip3 -v install docker-compose
```

Reboot

```sh
sudo reboot
```
