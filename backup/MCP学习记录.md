气死我了，写了一半重启电脑忘记保存了！
# MCP
  今天主要了解了这个东西，MCP 全称Model Context Protocol，模型上下文协议，名字起得其实不错，就是给模型装上手脚的感觉，目前的感觉是这个手脚接的比较随便，意思是说接上去比较容易，什么样的手脚都好接，但是接上之后的效果不是那么浑然一体，耗时略长。当然总体还是非常棒的！
  试用方式是用vscode中的Cline插件（它的MCP调用逻辑是把内容一股脑加入系统提示词，5fire的逻辑是要求模型支持function call，which，我不大清楚，大致就是模型选择方法来调用的一种内置功能吧），接了DEEPSEEK的付费API，openrouter的免费API好像始终不成功，然后就可以直接往MCP server里面配置MCP 组件了，配置方式还是比较简单的。（我是跟着这个up来做的https://www.bilibili.com/video/BV1AnQNYxEsy/?spm_id_from=333.1387.upload.video_card.click）
  总体理解下来觉得和模型训练相比，接手脚虽然对用户使用体验的影响似乎更大，但是背后的逻辑远没有模型训练复杂，甚至还比较好理解，拿github mcp举例，用户输入之后，给API发送的message除了question之外，还有固定的system prompt（就是字符串，里面有什么内容取决于你配置了哪些MCP组件），然后模型就知道具体调用哪个文件的哪个方法来获取信息/或者是直接进行一些操作（这些权限都有可视化界面设置，我觉得设计得挺好的），调用的过程基本上就是cmd调用nodejs程序。
  但是我现在有一个困惑就是怎么把这种能力加入到自己的代码里，中间的过程不是完全理解，使用过程感觉完全依赖客户端了，不管是Cline还是cherry studio。先继续了解吧，熟悉的MCP功能多一些、深入一些了或许会有些不同。实在不济，作为一个几乎全能全知的客户端也还是不错的，它甚至可以直接在桌面上创建编辑文件吧。
![Image](https://github.com/user-attachments/assets/b97fe597-071d-4104-b6bc-70b40b3f5311)
# Cursor
AI编程的尝试了vscode里面的roo code，cursor里面配自己的API有点麻烦，倒也是配置好了，但是现在感觉使用还不是很习惯。
# 宝塔
把模板文件放进去了，网页内容怎么不更新，试了两遍都是一样，不理解不理解。
 