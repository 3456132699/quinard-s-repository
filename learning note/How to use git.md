# 初始化
1. 找到文件夹
     `cd "E:\vs code\markdown"`
     >注意文件地址需要用引号
    1. 初始化，创建git文件
    `git init`

# 功能性代码
1. 查看文件状态
    `git status`
    2. 保存用户名称和邮箱（注意空格）
    `git config --global user.name "quinard"`
    `git config --global user.email "3456132699@qq.com"`
    用此查看是否成功
    `git config --global --list`
1. 清屏
    `clear`

# 保存到git
1. 进入缓存区(以test.md为例)
    `git add test.md`
2. 进入到commit历史
    `git commit -m "此处可以添加每一个commit的说明"`
    >此代码是把暂存区所有的代码都提交
3. 查看commit历史
    `git log`

# 三种回滚操作
1. 在工作区
     - **status回车后的含义**
      staged在暂存区内
    not staged尚未暂存，还在工作区 
    nothing to commit, working tree clean说明没有修改
 - 查看修改内容
   `git diff`
   |按键|功能|
   |:---:|:----:|
   |j|下移|
   |k|上移|
   |f|下翻页|
   |g|上翻页|
   |**q**|==退出此页面==|
  
- 撤销修改
  `git restore test.md`
  `git resore .`
  > .表示回滚一整个目录
2. 在暂存区
   - `git restore --staged .`
 >.的意思是把整个目录都选上
 >这只是撤销暂存当前的预览界面（工作区）做出的修改仍然存在
3. 在commit历史区
    -`git reset --hard HEAD~1`
    >HEAD表示最新的commit，HEAD~1则是其下一个，那么这个代码表示把HEAD的位置往下变成HEAD~1，所以原来最新的文件就消失了

    ![pnU2OVU.jpg](https://s41.ax1x.com/2026/10/11/pnU2OVU.jpg)


# 忽略文件
 `vim .gitignore`
 >回车后会出现一个特殊页面，要先点i才能打字，在里面输入文件名（注意要加后缀），就能忽略文件，让git不管他了。
  >在点击Esc,点:wq,回车，就能保存退出
  >应该把.gitignore也提交到commit区

# 如何使用GitHub
1. 配置ssh key
     `ssh-keygen -t ed25519 -C "mark.3456132699@qq.com"`
     >接下来全点回车，存储位置默认，密码不用设置
2. 显示公钥
    `cat ~/.ssh/id_ed25519.pub`
    把显示的公钥添加到GitHub即可
3. 检测是否生效
    `ssh -T git@github.com`这是尝试连接
    >连接成功后，点yes回车

# 创建GitHub仓库
 - 上传文件
 `git push`
  >可以把commit历史区的文件全部同步推送到GitHub上
- 下载文件
  `git clone git@github.com:3456132699/quinard-s-repository.git 哈哈哈哈`
  >那一大长串是从GitHub仓库code——ssh复制下来的，空一格加文件夹的名称

# GitHub使用
### 快捷键
/ 搜索   
t 定位到文件搜索   
l 跳转行数










 
  [![pnUfWVK.png](https://s41.ax1x.com/2026/10/11/pnUfWVK.png)](https://imgchr.com/i/pnUfWVK)
[![pnUf2b6.png](https://s41.ax1x.com/2026/10/11/pnUf2b6.png)](https://imgchr.com/i/pnUf2b6)