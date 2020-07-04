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

apt install nodejs-legacy -y

apt install npm -y

npm update

reboot

----------------------------------------------------------
__________________________________________________

OLD VERSION NOMPIX11 u16
______________________________________________________

cd nomp

sudo apt install npm -y

sudo npm install posix -y

curl https://raw.githubusercontent.com/creationix/nvm/v0.16.1/install.sh | sh

source ~/.profile

nvm install 0.10.25

nvm use 0.10.25

---------------------------------------


cd $HOME/nomp

sudo ufw allow 3011/tcp

sudo ufw allow 3012/tcp

sudo ufw allow 8013/tcp

______________________________________________________
RUN

nvm use 0.10.25

npm rebuild

npm update

node init.js

______________________________________________________

close node all

killall node











