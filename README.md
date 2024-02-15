## ===== Install / Update SKYCOIN  =====
## Buka Aplikasi SSH Lanjut Paste

1. (A). Install skywire
## sudo dpkg -i $(curl -L https://github.com/skycoin/apt-repo/releases/download/current/skybian-$(dpkg --print-architecture).deb -o skybian-$(dpkg --print-architecture).deb && echo -e skybian-$(dpkg --print-architecture).deb) && rm skybian-*.deb && install-skywire

1. (B) atau jika error (Update skywire)
## sudo dpkg -i $(curl -L https://github.com/skycoin/apt-repo/releases/download/current/skyrepo-$(dpkg --print-architecture).deb -o skyrepo-$(dpkg --print-architecture).deb && echo -e skyrepo-$(dpkg --print-architecture).deb) && sudo rm skyrepo-*.deb && sudo install-skywire || apt install skywire-bin


2. set your reward address
## skywire-cli reward <skycoin-wallet-address>
example :  skywire-cli reward vAVodsnSdqk94cX...............................
## Note : gunakan wallet skycoin di android klw sudah masuk baru kirim ke wallet exchanger (ex.LBank)
# Untuk yang belum daftar silakan daftar dlu : https://www.lbank.com/login/?icode=1EX6U


3. (A). set remote hypervisor (untuk Perangkat/estebe No. 1)
## skywire-autoconfig <hypervisor-public-key>
# contoh : skywire-autoconfig 0359486810616ba............................. 
# Note : dicopy dinotepad hypervisor-public-key 


3. (B). set remote hypervisor (untuk Perangkat/estebe No. 2,3,4,5 dst)
## skywire-autoconfig <hypervisor-public-key>
# contoh : skywire-autoconfig 0359486810616ba............................. 
# Note : pastekan hypervisor-public-key yang sudah dicopy 
