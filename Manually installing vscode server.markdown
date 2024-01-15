# Manually installing vscode server
手动安装步骤
## 预先创建文件夹，对应的${commit_id}需要替换成那串数字
mkdir -p ~/.vscode-server/bin/${commit_id}
 
## 进入到文件夹并下载依赖
cd ~/.vscode-server/bin/${commit_id}
## 这个国内镜像下载，注意Remote-SSH的版本，这里是stable. 也可以使用官方的地址
https://vscode.cdn.azure.cn/stable/${commit_id}/vscode-server-linux-x64.tar.gz
 
## 使用浏览器下载此文件再用FTP工具上传到服务器
 
## tar解压文件到当前的文件夹，因为之前已经cd，所以正好是vscode代码需要检索的地方
## 检测到有相应的东西，vscode就会跳过下载直接启动远程的终端及相应线程
tar zxvf vscode-server-linux-x64.tar.gz --strip 1
## 这个命令尤其重要否则会不成功
touch ~/.vscode-server/bin/${commit_id}/0