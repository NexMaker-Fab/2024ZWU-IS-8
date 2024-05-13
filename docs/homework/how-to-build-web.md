# 怎样建设一个网站

## 1. 准备
  
我们将使用以下工具来构建我们自己的网页：

- Git：用于控制我们在GitLab中的版本。（ps. 经验所言，Mac也是需要下载并安装的哦，同时在安装时，记得断网，不然会卡住的。)
- 使用GitHub作为我们网页的服务。
- GitHub桌面：方便我们将编码从本地传输到GitHub。
- 使用Node.js构建环境。
- 用于写文档的VScode。
- 撰写我们文档的Markdown语言。
- 图片上传服务，我们使用PicGo将我们的图片存储在云端（例如在GitLab），并在标记文档中使用。

## 2. 网页设置

### 创建GitHub存储库

首先，你需要在GitHub上创建一个新的存储库来托管你的网站。

1. 登录你的GitHub账号。
2. 创建一个公共存储库，然后您可以与您的团队一起创建web内容。  
    ![图片1](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/a876c079a624d3ce907da503803aa2150b97cf8d/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/1.png)
3. 给您的存储库命名，选择公共或私有。添加一个README文件来共享您的信息，然后单击“create repository”按钮。  
    ![图片2](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/a876c079a624d3ce907da503803aa2150b97cf8d/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/2.png)
4. 设置页面为空。单击存储库的设置，并选择左侧的“page”。选择“main”和“/root”并保存。上面的链接允许您查看该页。  
    ![图片3](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/a876c079a624d3ce907da503803aa2150b97cf8d/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/3.png)

### 邀请团队成员

1. 打开创建的存储库。    
   ![图片4](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/4.png)
2. 单击“设置”，在左侧找到“协作者”，然后单击“添加人员”，输入他们的电子邮件地址并设置他们的身份（maintain）。  
   ![图片5](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/5.png)  
   ![图片6](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/6.png)

### 网络上传

将存储库克隆到GitHub。

1. 点击“添加”，“克隆资源”，找到需要克隆的存储库。最后按一下克隆。  
   ![图片7](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/7.png)  
   ![图片8](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/8.png)

### Github桌面登录

1. 找到您的存储库，单击打开“在Visual Studio Code中打开”，在Visual Studio Code中输入新内容并保存。  
   ![图片9](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/9.png)
2. 文档更改后，在第一个框中输入任何内容，然后单击Commit to main，然后push origin，如果图标显示为循环，则同步成功。  
   ![图片10](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/10.png)  
   ![图片11](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/11.png)

### Docsify

打开VScode，新建终端。  
![图片12](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/12.png)

点开setting，找到developer setting，点击Tokens（classic）选择generate new token（classic）再在note中输入名称，将expiration改成想要的时间，然后将repo，workflow，write：packages全选上，生成密钥，然后复制。

1. 安装docsify：  
   `npm i docsify-cli -g`
2. 确定位置，然后初始化环境：  
   `docsify init ./docs`
3. 预览：  
   `docsify serve docs`
4. 浏览器访问：http://localhost:3000
5. setting index.html
6. write document
7. Save all document

### 图片上传

1. 安装Picgo
2. 在GitHub上新建图片仓库
3. 进入图床设置
4. 获取密钥
5. 设定自定义域名使用cdn加速https://cdn.jsdelivr.net/gh/用户名/图床仓库名，完成Picgo设置  
   ![图片13](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/13.png)  
   ![图片14](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/14.png)  
   ![图片15](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/15.png)
6. 点击图床设置，找到GitHub，将密钥复制到token上，其他的按要求填完。  
   ![图片16](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/16.png)
7. 接着将图片拖拽到上传区，在相册中查看是否上传成功，同时可以复制图片路径  
   ![图片17](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/17.png)  
   ![图片18](https://github.com/NexMaker-Fab/2024ZWU-IS-BUNBUN/raw/0f6d4c38c0192d8f96731a41af4871b3a96126f4/images/%E6%9C%AA%E5%91%BD%E5%90%8D%E6%96%87%E4%BB%B6%E5%A4%B9/18.png)
   (ps. 如果picgo配置一直失败，可以直接在Github仓库中创建存放images的文件夹，并Add file。)
