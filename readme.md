For old SHA/X11/OTHERS u16
______________________________________________________

git clone https://github.com/allforminers/nompix-16.git nomp

dd if=/dev/zero of=/mnt/myswap.swap bs=1M count=4000

mkswap /mnt/myswap.swap

swapon /mnt/myswap.swap

nano /etc/fstab

______________________________________________________


paste this *************

/mnt/myswap.swap none swap sw 0 0

______________________________________________________


git clone https://github.com/allforminers/installubuntu.git

cd installubuntu

sudo bash install.sh

cd ..

----------------------------------------------------------

cd nomp

apt-get install -y libboost-all-dev git npm nodejs nodejs-legacy libminiupnpc-dev redis-server -y

npm update

reboot

----------------------------------------------------------
how-to-install-node-js-on-ubuntu-16-04

https://www.digitalocean.com/community/tutorials/how-to-install-node-js-on-ubuntu-16-04



cd nomp

apt install curl -y

curl -sL https://raw.githubusercontent.com/creationix/nvm/v0.33.8/install.sh -o install_nvm.sh

bash install_nvm.sh

source ~/.profile

nvm ls-remote

nvm install 0.10.25

nvm use 0.10.25

sudo npm install posix -y
----------------------------------------------------------


cd $HOME/nomp

sudo ufw allow 3011/tcp

sudo ufw allow 3012/tcp

sudo ufw allow 3013/tcp

______________________________________________________
RUN

nvm use 0.10.25

npm rebuild

npm update

node init.js

______________________________________________________

close node all

killall node











