### 生成ssh的命令
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

### 获取ssh的命令
cat ~/.ssh/id_rsa.pub

### 本机电脑配置全局变量
git config --global user.name "example"
git config --global user.email "your_email@example.com"

### 将GitHub上的仓库下载至本机
git clone 仓库地址

### 本地仓库提交的步骤
git add -A
git commit -m "本次提交的修改的备注"
git push origin main（第一次提交）
git push（非第一次提交）

在协同开发时，每次提交前最好执行一次git pull

### 绑定本地仓库
1. 创建线上空仓库和本地同名新文件夹
2. 先后执行 git init 、 git remote add origin 仓库地址
3. git remote -v 查看绑定
4. git remote remove origin 移除绑定
