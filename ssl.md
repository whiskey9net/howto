### Configure OpenVPN
```
sudo apt-get update && sudo apt-get install openvpn easy-rsa

make-cadir certificates && cd certificates

vi vars

source vars

./clean-all && ./build-ca
./build-key-server server
./build-dh
openvpn --genkey --secret keys/ta.key
```
