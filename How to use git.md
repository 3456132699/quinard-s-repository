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
   >j下移  k上移  f下翻页  g上翻页 q退出此页面
- 撤销修改
  `git restore test.md`
  `git resore .`
  > .表示回滚一整个目录
2. 在暂存区
   - 

