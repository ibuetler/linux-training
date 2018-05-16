# Solution 02
## start the Hacking-Lab LiveCD in VirtualBox
* start VirtualBox
* start Hacking-Lab LiveCD
* login with username "hacker" and password "compass"
* open a shell
* find out ip address of your linux host (eth0)
```
ifconfig -a
```

## get and install putty on your Windows PC
* get the putty bundle from https://the.earth.li/~sgtatham/putty/latest/w64/putty-64bit-0.70-installer.msi
* install putty on your Windows computer

## ssh from Windows to Linux using putty
* open a cmd.exe (Windows + TAB and type putty) 
```
putty
```
* a graphical UI should appear; enter your linux ip address you got from the step above
* connect
* try the username and password of your linux account (hacker:compass)
* you should be logged in
* try the following linux commands
```
pwd
ls 
ls -al 
hostname
ifconfig -a
whoami
apt-get update
apt-get upgrade
apt-get dist-upgrade
```


## scp from Windows to Linux using pscp
* open a cmd.exe (Windows + TAB and type cmd)
* in cmd.exe type "pscp" and read the output
```
pscp
```
* create a test file on your Windows host and add some text in it, save and close notepad
```
notepad text.txt
```
* in your cmd.exe type 
```
pscp.exe test.txt hacker@ip-address-of-your-linux:
pscp.exe test.txt -l ip-address-of-your-linux:
```

## scp from Linux to Windows using pscp
* open a cmd.exe (or use the cmd.exe that is still open)
* delete the test.txt with
```
del test.txt
```
* in cmd.exe type the following commands
```
pscp.exe -l hacker ip-address-of-your-linux:test.txt .
pscp.exe ibuetler@ip-address-of-your-linux:test.txt .
```

