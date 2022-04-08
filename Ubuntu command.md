## SCP from a remote machine to your machine
```bash
scp ${user_name}@${ip_address}:/${absolute_path} ${local_path}
```   
    
    
## Look at disk capacity
```bash
du -h /disk1 | sort -h
df -h --total
```
- h -> display storage in MB/GB instead of bytes
- /disk1 -> name of the disk you want to see
- sort -> going to display relative to the size

## Untar a file to a folder
```bash
tar -czvf ${tar_file} ${folder_name}
```
    
## Make a file with a specific size
```bash
truncate -s ${size}(100k) ${filename}
```
    
## Get unix timestamp
```bash
DATE="22-sEP-2014 10:32:35.012"
date -d "$DATE" +'%s/$3N'
```
    
## 查看包括ssh上的所有进程
```bash
ps aux
```
    
## 看到所有环境变量  
```bash
env
```
    
## 找文件
```bash
find -iname ${文件名}
```
    
## Let terminal forget previous remembered path
```bash
hash -r
```
    
## htop
```bash
sudo apt-get install htop
方便看到电脑状态
```
    
## screen
```bash
sudo apt-get install screen
# 可以让程序在后端跑
screen -r # 可以看到自己的进程

#screen 在.sh文件开启方法
第一行加#!/bin/bash
screen -Sdm start_rviz $I3dLoc/bin/enable_rviz.sh #或者直接roslaunch
echo "Enable RVIZ"
sleep 5

# screen 删除script
#!/bin/bash
pkill screen
```
  
## Tmux
```bash
sudo apt-get install screen
开了tmux之后，就不必在乎ssh断开，会在后台跑
tmux attach可以看到后台的
```
    
## Fix ssh problem
Face the problem "REMOTE HOST IDENTIFICATION HAS CHANGED!" Add correct host key in ...

```bash
ssh-keygen -R "$ip-address"
```
## Check dependencies version
```bash
dpkg -s "$dependencies-name" | grep 'Version'
```


## 更新一个文件的时间，可以重新make (或者在编译一次）
```bash
touch ${filename}
```
