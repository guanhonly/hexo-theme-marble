## hexo-theme-marble

#### 新个人博客地址：[Honly's blog](https://guanhonly.github.io/)
* * *
#### 自己动手做的一个github个人主页，在[@ppoffice](https://github.com/ppoffice)的[Alex](https://github.com/ppoffice/hexo-theme-alex)项目基础上改的，主要是根据我的个人喜好进行的界面的调整，增加了评论功能。评论功能采用的[gitalk](https://github.com/gitalk/gitalk)。

## 安装方法：
#### 1. nodejs和hexo的安装可以参考这篇博客：
> [用Hexo + github搭建自己的博客 --- 再也不用羡慕别人了！
](https://blog.csdn.net/Hoshea_chx/article/details/78826689)

#### 2. 在你新建的hexo目录下，安装这个主题：
```
git clone https://github.com/guanhonly/guanhonly.github.io.git themes/marble
```
marble要求Hexo 2.4及以上版本

#### 3. 更改clone后的marble中的`_config.yml`，相关参数可见[Alex](https://github.com/ppoffice/hexo-theme-alex)的文档

#### 4. gitalk相关配置
* 首先，去[这里](https://github.com/settings/applications/new)申请github的授权，获得client ID和client Secret。
* 然后，修改 `_config.yml`中的相关配置：
> gitalk:
  enable: true
  language: # 指定语言，默认从系统中获取
  owner: # 申请时的owner
  admin: # 管理员，如果没有其他人，填自己
  github_repo: # 用与保存评论的仓库名，建议填个人主页对应的仓库
  client_id: # 刚刚生成的client ID
  client_secret: # 刚刚生成的client Secret

#### 5. 在个人主页的根目录下，运行
```
hexo clean
```
#### 然后运行
```
hexo g
```
#### 最后运行
```
hexo d
```
过一会儿就可以上看到使用了这个模板的个人主页了

效果：
![](https://raw.githubusercontent.com/guanhonly/HonlyBlogHelper/master/images/oldBlog1.png)
![](https://raw.githubusercontent.com/guanhonly/HonlyBlogHelper/master/images/oldBlog2.png)