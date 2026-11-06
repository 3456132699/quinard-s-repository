# 开发环境配置

###  anaconda和conda
- **conda**：管家。专门管两件事：新建互相隔离的房间（虚拟环境）、在房间里安装 / 卸载工具包。
- **Anaconda**：一整套打包好的大工具箱套装，里面自带了 conda 这个管家，还预装了 Python、一堆常用代码库、Anaconda Prompt 窗口。

### 配置环境变量
环境变量就是操作系统里一张 “全局小纸条”，上面记着一些路径、参数；配置环境变量，就是修改这张纸条，让系统能找到你想用的程序。
>> 1. **系统 PATH（永久配置，控制面板里改的那种）**
一旦添加，所有 CMD、PowerShell 窗口都能识别`conda`命令；缺点是容易冲突，很多教程不推荐直接勾这个。
>>2. **临时环境变量（Anaconda Prompt 自动加载）**Anaconda Prompt 本质是一个**定制启动器**：它启动的时候，自动运行一段脚本，把 conda、python、pip 所在文件夹路径，临时加到这个窗口内部的 PATH 里。
✅ 只对**当前这一个黑窗口生效**；关掉窗口，这些临时添加的路径就消失了，不会改动电脑系统设置。
所以你打开它直接敲 `conda`、`pip`，系统找得到程序，**看起来就像 “不用配环境变量”**
### pip
p 是 Python 自带的「零件采购员」，只管安装 Python 的第三方代码包。

### anaconda power shell prompt 和 anaconda prompt 有什么区别
anaconda power shell prompt 和 anaconda prompt 有什么区别
1. **Anaconda Prompt**：底层是老旧 CMD（cmd.exe）
2. **Anaconda PowerShell Prompt**：底层是 PowerShell



# Jupyter notebook基本使用
### 单元格类型
每个单元格都有一个类型，可以是代码单元格（Code）、标记单元格（Markdown）或文本单元格（Raw）。代码单元格用于编写和执行代码，标记单元格用于使用Markdown语法添加格式和标记，文本单元格用于编写解释性文本。

