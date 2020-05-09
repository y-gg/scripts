# scripts
1、将pre-receive和post-receive两个文件拷贝到编译服务器（Linux）源码目录src/.git/hooks/  
并修改文件权限 
```
cd src/.git/hooks/  
chmod 755 pre-receive post-receive
```
修改git配置允许更新当前分支  
```
git config receive.denyCurrentBranch warn
```
2、开发环境（Windows）下源码添加编译服务器地址ip:/home/src or name@ip:/home/src
```
cd HwPkg
git remote add local name@ip:/home/src
```
