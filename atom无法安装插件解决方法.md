#### 1.安装Node.js
  因为在安装atom插件的时候，需要用到Node.js的npm命令，所以先安装Node.js，配置好环境环境（默认安装完成后会自动配置好）。

  在cmd中输入：node --version,检查环境变量是否配置成功

#### 2.下载需要的插件到C:\User\用户名\.atom\pacages目录下
* 打开 https://atom.io/packages 网址，查找所需要的插件。
* 选择插件中的repo，复制github地址。
![](https://raw.githubusercontent.com/meiSThub/AtomProject/master/image/pg_1.jpg)
* git clone https://github.com/cakebake/markdown-themeable-pdf.git （将插件的源代码克隆岛文件夹中）
* cd markdown-themeable-pdf （进入插件包文件夹）
* npm install （下载，生成插件）

#### 3.重启atom 或者 control + alt + R 刷新atom
