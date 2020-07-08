
1. Install Docker
curl -sSL https://get.docker.com | sh

2. Add permission to Pi User to run Docker Commands
sudo usermod -aG docker pi

Reboot here or run the next commands with a sudo

3. Test Docker installation
docker run hello-world

4. IMPORTANT! Install proper dependencies
sudo apt-get install -y libffi-dev libssl-dev

sudo apt-get install -y python3 python3-pip

sudo apt-get remove python-configparser

5. Install Docker Compose
sudo pip3 -v install docker-compose



Linux下更换镜像源
修改 ~/.pip/pip.conf 文件, 没有则创建
[global]
timeout = 6000
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
trusted-host = pypi.tuna.tsinghua.edu.cn
