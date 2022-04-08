## 一、安装前的准备
```bash
sudo apt install ibus-rime（安装rime输入法）
sudo apt install librime-data-pinyin-simp （安装简体拼音库）
```

## 二、设置自定义文件
在 `~/.config/ibus/rime/` 下新建一个文件  `default.custom.yaml` （覆盖默认设置）
```bash
$ ls -lSh  ~/.config/ibus/rime | sed "s/$USER/me/g"
total 32K
drwxrwxr-x 2 me me 4.0K May 14 12:15 build
drwxr-xr-x 2 me me 4.0K May 14 12:45 luna_pinyin.userdb
drwxr-xr-x 2 me me 4.0K May 14 11:14 pinyin_simp.userdb
drwxrwxr-x 3 me me 4.0K May 14 08:59 sync
-rw-rw-r-- 1 me me  202 May 14 08:58 installation.yaml
-rw-r--r-- 1 me me  120 May 14 12:12 default.custom.yaml
-rw-r--r-- 1 me me   74 May 14 11:36 #default.custom.yaml#
-rw-rw-r-- 1 me me   34 May 14 12:15 user.yaml
-rw-r--r-- 1 me me    0 May 14 09:33 default.custom.yaml~
```
自定义文件的内容

```bash
$ cat ~/.config/ibus/rime/default.custom.yaml
patch:
  style/horizontal: true  #无效的设置
  schema_list:
    - schema: luna_pinyin_simp
  style:
    - horizontal: true  #无效的设置
```

## 三、重启系统， 使安装生效

## 四、调出Chinese(Rime)
打开“setting（设置）”, “Region&Language（区域和语言）”，点+号, 添加输入法 Chinese(Rime) 。如果不用其它输入法，可以删除，其实也真不用其它输入法了.

## 五、部署
系统右上角选择输入法， 下拉部署