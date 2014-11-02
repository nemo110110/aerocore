#Nuttx developed Kit#

-----
Environment

* sudo apt-get install python-serial python-argparse openocd \
    flex bison libncurses5-dev autoconf texinfo build-essential \
    libftdi-dev libtool zlib1g-dev genromfs git-core wget


-----
Arm-none-eabi-gcc
pushd .
cd ~
wget https://launchpadlibrarian.net/174121628/gcc-arm-none-eabi-4_7-2014q2-20140408-linux.tar.bz2
tar -jxf gcc-arm-none-eabi-4_7-2014q2-20140408-linux.tar.bz2
exportline="export PATH=$HOME/gcc-arm-none-eabi-4_7-2014q2/bin:\$PATH"
if grep -Fxq "$exportline" ~/.profile; then echo nothing to do ; else echo $exportline >> ~/.profile; fi
. ~/.profile
popd


. ~/.profile


export PATH=$HOME/gcc-arm-none-eabi-4_7-2014q2/bin:\$PATH

source ~/.bashrc


----
ST-Link
git clone https://github.com/texane/stlink
