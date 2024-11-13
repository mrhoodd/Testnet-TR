-------------------------------------- Servisli-----------------------------
```
cd
systemctl stop pactusd
wget https://github.com/pactus-project/pactus/releases/download/v1.5.0/pactus-cli_1.5.0_linux_amd64.tar.gz
tar -xvf pactus-cli_1.5.0_linux_amd64.tar.gz
cp -r pactus-cli_1.5.0/* pac/
systemctl restart pactusd
```
```
journalctl -u pactusd -fo cat
```

-------------------------------------- Manuel -----------------------------
```
cd
wget https://github.com/pactus-project/pactus/releases/download/v1.5.0/pactus-cli_1.5.0_linux_amd64.tar.gz
tar -xvf pactus-cli_1.5.0_linux_amd64.tar.gz
```
### Screen'e girelim. 
```
screen -r pactus
```
##### Ardından CTRL+C ile durduralım.
```
cd
cd pactus-cli_1.5.0
```
```
./pactus-daemon start -w ~/pactus
```
