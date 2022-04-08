```bash
1.安装的时候不需要连接网络，然后不要安装第三方的driver
2.sudo apt-get update && sudo apt-get upgrade
3.找到需要的cuda driver版本，执行所有的步骤（除了sudo apt-get install cuda）
4.ubuntu-driver devices
5.安装合适的版本sudo apt install nvidia-driver-460（xxx）合适的版本
6.sudo apt-get install cuda-toolkit-10-2(xx-x) 合适的版本
7.cd /usr/local && sudo rm cuda && sudo ln -s cuda-10.2（x.x） cuda 和6一样的版本
```