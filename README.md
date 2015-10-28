# lightcloud
##简介
这是一个轻量化的简洁风格的Ghost主题，参考ghostchin.com网站外观编写，基于国内的开源前端框架[AmazeUI](http://amazeui.org/)开发。  
点击这里查看[Demo](http://xknow.net)。

##特点
* 精简风格
* 响应式布局
* 支持分享文章到新浪微博和QQ空间
* 支持多说社交化评论

##安装
git用户直接克隆仓库即可  
`git clone https://github.com/microud/lightcloud.git`  

非git用户可下载zip压缩包并解压  
将文件夹复制到ghost目录下的`content/themes`目录，然后重启ghost即可。

##配置
###post.hbs
注释标注处可将js换为自己的多说提供的js代码。

###sidebar.hbs
* 关注模块：可以自行添加删除图标，修改“a”标签链接使之指向自己的公众页面。
* 友情链接：可以自行复制原有的模板代码修改链接添加。
* 标签云：需要对应的模块支持，如果使用的是[ghost中文网](http://ghostchina.com)中的中文版ghost，则不需要进行多余的配置，如果是英文版则需要根据以下步骤添加模块。  

> 将仓库中tag_cloud目录中`tag_cloud.js`的复制到`core/server/helpers/`中，子目录tpl中的`tag_cloud.hbs`复制到对应的子目录tpl中。

> 修改`core/server/helpers/index.js`，参考https://github.com/ghostchina/Ghost-zh/blob/master/core/server/helpers/index.js  添加两行代码。

> 重启ghost

> 更多详细步骤可参考官方博客http://www.ghostchina.com/output-tag-cloud/
