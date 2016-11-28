
# 基本命令
***
#### 目录/文件的操作
* mkdir "目录名"             在当前路径下创建一个文件夹  
* mvdir "目录1" "目录2"      移动或者重命名一个目录    (如果目录2不存在,就直接修改目录1的名称为目录2)  
* rmdir "目录名"             删除一个目录    
***
#### 转换目录

* cd + "路径"           进入该文件目录下(也可以将文件直接拖进来)

* cd ..                回到上级目录

* cd .                 当前目录

* cd /                 回到根目录

* cd test.rtf 不可用. 不能cd到文件里.只能cd到目录.  -bash: cd: test.rtf: Not a directory
***
#### 拷贝/移动/删除
* cp "需要拷贝的文件路径" "目标地址路径"     拷贝文件   例如: cp /Users/goulela/Desktop/test.rtf /Users/goulela/Desktop/文件夹2

* mv "需要移动的文件路径" "目标地址路径"     移动文件        例如: * mv 文件夹2 /Users/goulela/Desktop/创建文件夹/文件夹

* rm "路径"            删除文件           参数－rf 表示递归和强制，千万要小心使用，如果执行了 rm -rf / 你的系统就全没了
***
#### 创建并编辑文件
* cd 到想要创建文件的路径下 
* vim "文件名.txt(需要加上想要创建的文件后缀,自动生成该后缀类型的文件)" 
 
***
### 显示操作
* file "文件名"        显示文件的类型 
* wc   "文件名"        统计文件的字符数,词数,行数

* pwd                 查看当前所在的目录

* ls                  显示当前路径下有什么文件
* ls + "目录名"        显示特定的路径下有什么文件
* ls -w               显示中文
* ls -l               详细信息
* ls -a               包括隐藏文件


### 时间操作
* date                显示系统的当前日期和时间
* cal                 显示日历


### 网络与通信
* ping ""url"        给一个远程主机发送 回应请求 
* 终止ping打印         control + c
* who                列出当前登录的所有用户
* whoami              显示当前正进行操作的用户名

# Git命令
### 1.服务器拉取代码
* git clone "url"         说明:url为服务器地址,用https的地址
### 2.本地代码上传服务器
* (最简单的方法)先在服务器上创建好项目,然后clone到本地,然后把项目copy进去.
* (严格的方法) cd 到该项目的路径下
*  git init
*  git add .
*  git remote add origin "url" 
*  git commit -m "你的本次提交的备注信息"
*  git pull
*  git push 
### 3.查看命令
* git status            查看当前git的状态(未拉取的提交,和本地未提交的版本)
* git log                
* git show
* git diff
* git config 
### 提交命令
* git add "文件名"
* git add .
* git pull
* git push    
  
### 分支操作

### gitignore的使用

### 如何切换不同的服务器


后续补充中...