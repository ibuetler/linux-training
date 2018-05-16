# Solution 02
## get and install putty on your Windows PC
* get the putty bundle from https://the.earth.li/~sgtatham/putty/latest/w64/putty-64bit-0.70-installer.msi
* install putty on your Windows computer

## ssh from Windows to Linux
* open a cmd.exe (Windows + TAB and type cmd)
* type "putty" followed by ENTER
* enter your linux ip address
* connect
* try the username and password of your linux account (hacker:compass)


## scp from Windows to Linux
* open a cmd.exe (Windows + TAB and type cmd)
```
pscp
```
* create a test file and add some text in it, save and close notepad
```
notepad text.txt
```
* in your cmd.exe type 
```
pscp.exe test.txt hacker@ip-of-your-linux:
```
