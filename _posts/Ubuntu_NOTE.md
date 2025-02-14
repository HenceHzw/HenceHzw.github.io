# ubuntu系统

## 安装压缩包

```
sudo dpkg -i wps-office_12.1.0.17885_amd64.deb 
tar -xvf cudnn-linux-x86_64-8.9.7.29_cuda12-archive.tar.xz
tar zxvf cudnn-11.1-linux-x64-v8.0.4.30.tgz
```

## 删除软件

```
#通过.deb安装的
sudo apt remove obsidian     
sudo apt purge obsidian       //彻底删除，包括配置文件

rm -rf ~/.config/obsidian     //进一步删除
rm -rf ~/.obsidian

dpkg -l | grep obsidian       //输出为空，即已删除
```

## 终端输出写入文件

```
nohup ./OpenCV_Project
```

## 海康MVS

```
cd /opt/MVS/bin
./MVS.sh
```

## 复制终端文件到本地

```
scp -rP 35394 root@region-1.autodl.com:/实例中/某个文件或文件夹 <本地文件/文件夹> （注意需要在本地的机器上执行）
 scp -rP 26304 root@connect.cqa1.seetacloud.com:/root/autodl-tmp/results_attention "E:/Research_Learning/Temporary transfer station"


scp -rP 10350 root@connect.nmb1.seetacloud.com:/root/autodl-tmp/Results/outputs/original_model/checkpoints "/media/hence/E/Research_Learning/Temporary transfer station/checkpoints/original"


本地到终端
sudo scp -r -P 10350 /home/hence/文档/cat2dog rootconnect.nmb1.seetacloud.com:/root/autodl-tmp/Dataset
```

## root身份打开根目录

```
sudo nautilus
```

## 查找文件

```
find 搜索路径 -type d -name "文件夹名"
find . -type d -name "myfolder"     在当前目录及其子目录中查找名为 myfolder 的文件夹 
find / -type d -name "myfolder"     在整个系统中查找名为 myfolder 的文件夹
```

## 统计文件夹中文件数量

```
find /path/to/directory -maxdepth 1 -type f | wc -l     # 仅统计文件数量（排除子文件夹）
# -maxdepth 1 仅搜索当前文件夹，不递归子文件夹。
# -type f 仅统计文件，排除文件夹。

# ls /path/to/directory | wc -l  #统计文件夹中的所有文件和子文件夹
```



# Python相关

## 列出库依赖

```
pip install pipreqs
pipreqs /home/hence/script    #在指定文件夹中生成requirements.txt文件
pip install -r requirements.txt      #安装所需依赖项
```

# 其他

## 启动ROS主节点  ROS Master

```
roscore
```

## GPT快捷键

```
Ctrl + ？   # 打开快捷键帮助
```

## github提交

```
# 上传到main主分支
git add .
git commit -m "your commit message"
git push origin main

# 上传到branch分支

```

## 本地项目上传到github仓库

```
--- HTTPS协议 ---
cd /path/to/your/project  # 进入你的项目目录
git init                 # 初始化 Git 仓库
git add .                # 添加当前目录下的所有文件到暂存区
git commit -m "Initial commit"  # 提交到本地仓库，附上提交信息

rm -rf .git      #删除本地仓库的Git信息，即将本地目录从Git仓库转换为普通文件夹

登录 GitHub
点击右上角的 "+" 按钮，选择 New Repository
输入仓库名称（如 my-project），选择公开或私有，点击 Create repository
仓库创建完成后，你会看到一个远程仓库的地址，如：https://github.com/your-username/my-project.git

#将你本地的 Git 仓库与远程仓库绑定
git remote add origin https://github.com/your-username/my-project.git  

#检查绑定是否成功
git remote -v   

#如果看到类似内容，则绑定成功
origin  https://github.com/your-username/my-project.git (fetch)   
origin  https://github.com/your-username/my-project.git (push)

git branch -M main    # 确保当前分支名称是 "main"（或根据需要更改为 "master"）
   # 将代码推送到远程仓库的 "main" 分支
（如果是第一次推送，git 可能会要求你输入 GitHub 的用户名和密码，见下面“git clone 私有库”）

--- HTTPS转SSH ---

```

## Branch提交

```
git fetch --all      #从远程仓库拉取所有分支


git branch    查看当前分支
git checkout <branch-name>     切换到目标分支
git pull origin <branch-name>     拉取分支代码


git add .
git commit -m "描述你的更改"    
git push origin <branch-name>
```

## Labelme

```
conda activate labelme
labelme
```

## 查看环境命令

```
env
或者
printenv
```

## 设置全局代理

```
git config --global http.proxy http://127.0.0.1:7897
git config --global https.proxy http://127.0.0.1:7897

禁用代理
git config --global --unset http.proxy       
git config --global --unset https.proxy
```

## git clone 私有库

```
settings -> developer settings -> Personal access tokens 
账号即邮箱 ，密码为Personal access tokens  
```
