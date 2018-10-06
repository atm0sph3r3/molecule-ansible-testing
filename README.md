$ sudo yum install -y yum-utils device-mapper-persistent-data lvm2

$ sudo yum-config-manager     --add-repo     https://download.docker.com/linux/centos/docker-ce.repo

$ sudo yum install docker-ce

$ sudo systemctl start docker

$ sudo systemctl enable docker

$ sudo docker run hello-world

$ curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py"

$ sudo python get-pip.py 

$ sudo pip install virtualenv

$ python -m virtualenv molecule-testing

$ cd molecule-testing/

$ source bin/activate

$ sudo yum install -y gcc python-devel

$ pip install molecule docker

$ molecule init role -r httpd -d docker

$ sudo usermod -aG docker vagrant

$ exit

$ sudo cp -r /usr/lib64/python2.7/site-packages/selinux ../lib/python2.7/site-packages/

$ molecule test
