# How to Linux Terminal
_by @AzureOrange and @RickDangerous_

This guide provides a list of useful shell commands to use inside RetroPie

1. Print current working directory  
```
pwd
```
2. change working directory  
```
cd /PATH/TO/DIRECTORY
```
3. list files inside working directory   
```
ls
```
4. list files including file permissions
```
ls -l
```
5. list files including hidden
```
ls -a
```
6. create new directory
```
mkdir
```
7. remove file
```
rm /PATH/TO/FILE
```
8. remove directory
```
rm -rf /PATH/TO/DIRECTORY
```
9. edit file using nano (Text editor)
```
nano /PATH/TO/FILE
```
10. shutdown immediately
```
sudo shutdown -h now
```
11. reboot
```
sudo reboot
```
12. Raspi-Config
```
sudo raspi-config
```
13. RetroPie Setup
```
sudo ~/RetroPie-Setup/retropie_setup.sh
```
14. network information
```
ifconfig
```
15. check CPU temperature
```
vcgencmd measure_temp
```
16. change owner of directory and all files in it recursively to user:group Pi
```
sudo chown -R pi:pi /PATH/TO/DIRECTORY
```
17. make file executable (mostly shell scripts)
```
sudo chmod +x /PATH/TO/script.sh
```
