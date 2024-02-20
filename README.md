#### Latest Ubiquity Unifi Controller 8.0.28 for Debian Bookworm on arm64 architecture!

Install required packages before you begin with the following command: 
```
sudo apt-get update && sudo apt-get install ca-certificates apt-transport-https
```
Use the following command to add a new source list: 
```
echo 'deb [ arch=amd64,arm64 ] https://www.ui.com/downloads/unifi/debian stable ubiquiti' | sudo tee /etc/apt/sources.list.d/100-ubnt-unifi.list
```
Install the following trusted GPG key into /etc/apt/trusted.gpg.d:
```
sudo wget -O /etc/apt/trusted.gpg.d/unifi-repo.gpg https://dl.ui.com/unifi/unifi-repo.gpg
```
get and install with dpkg or apt:
```
wget http://ports.ubuntu.com/pool/main/o/openssl/libssl1.0.0_1.0.2g-1ubuntu4_arm64.deb -O libssl1.0.deb
```
get and install with dpkg or apt:
```
wget https://repo.mongodb.org/apt/ubuntu/dists/xenial/mongodb-org/3.6/multiverse/binary-arm64/mongodb-org-server_3.6.22_arm64.deb -O mongodb.deb
```
install unifi controller package
```
sudo apt install unifi
```

Enjoy unifi network controller on arm64 :-)
