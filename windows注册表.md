右键添加Git Bash Here
第一步，window + R，输入regedit回车进入注册表
依次进入HKEY_CLASSES_ROOT —-》 Directory —-》Background —-》 shell
右键点击shell，选择新建，然后选择项，命名为 Git Bash Here，成功后进入桌面右键发现多了 Git Bash Here.
添加图标：右键点击shell中你刚刚新建的这个项(Git Bash Here)，选择新建，然后选择字符串值，将名称设置为Icon；
然后找一下你安装Git的文件夹，我是安装在了D盘，D:\Git\mingw64\share\git，按照这个路径进入到git文件夹，会发现里面有个git-for-windows.ico；然后将刚刚新建的字符串值的数据设置为D:\Git\mingw64\share\git\git-for-windows.ico；保存发现右键Git Bash Here中多了一个图标；
.
接下来还差最后一步，在 Git Bash Here 下面新建一个项(我的是git bash here，当时新建的时候没大写，不过问题不大)，名字为command


将数据设置成 D:\Git\bin\bash.exe –login -i，这个也和你安装Git的路径有关，我是安装在了D盘；