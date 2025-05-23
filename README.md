# Git学习笔记

## 学习资料链接
- [Git学习资料1](https://blog.csdn.net/mukes/article/details/115693833)
- [Git学习资料2](https://blog.csdn.net/m0_73972962/article/details/145406846)
- [Git学习资料3](https://blog.csdn.net/TroyeSivanlp/article/details/121172010)
- [Git学习资料4](https://blog.csdn.net/qq_29493173/article/details/113094143)
- [Git学习资料5](https://blog.csdn.net/ingenuou_/article/details/107452638)
- [Git学习资料6](https://blog.csdn.net/qq_29493173/article/details/113094143)
- [Git学习资料7](https://blog.csdn.net/li1325169021/article/details/140958106)
- [Git学习资料8](https://blog.csdn.net/G_matinal/article/details/137794921)
- [Git学习资料9](https://gitwebcn.com/26675.html)

## 学习流程

### 一. 安装和配置Git，创建本地仓库

1. **安装Git**: 从 [git官网](https://git-scm.com/) 下载并安装。
2. **配置Git**:
   打开bash，设置Git的用户名和邮箱：
   ```bash
   git config --global user.name "Name"
   git config --global user.email "xxxxx.com"
   
### 二.注册远程仓库账号并创建公开仓库
1. **注册远程仓库账号**:在GitHub注册一个账户。  
难点：邮箱收不到验证码  
解决方法：在邮箱“反垃圾”界面设置白名单
2. **创建远程仓库**:登录后，点击“New Repository”创建仓。
3. **进行ssh连接**：将C盘的.ssh文件里的公开链接添加到github。
4. **将本地仓库连接到远程仓库**:
git remote add origin git@github.com:xxx/xxx.git  
检查连接：git remote -v
5. **推送本地代码到远程仓库**:git push -u origin master
- 难点①：连接好之后代码推送不上去   
解决：最开始是通过http连接，因为网络问题无法推送。后来通过ssh连接就能成功推送。  
- 难点②：在上一级目录下进行的推送，导致该很多不需要上传的文件都被推送了。  
解决：在github上将仓库删除，将错误目录的.git文件删除。重新在正确的文件目录下进行推送。

### 三.提交至少三次代码并观察变更
**第一次**：只提交了svm.py  
**第二次**：提交打包好的c语言作业代码文件夹  
**第三次**：提交python和数据结构的作业文件代码  
![屏幕截图 2025-05-13 201001](https://github.com/user-attachments/assets/be35e859-994c-4fce-b987-fc3b97f5bdb6)
