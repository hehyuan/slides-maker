# Slide online.
这是可以通过写简单的`.md`文件就完成slides的制作的工具. 并且借助github的pages功能, 我们可以很方便地将其部署在静态网页上. 

## 部署步骤 
- 写完PPT, 也就是`slides.md`文件 
- 修改`package.json`文件中的name和build两个属性, 将其改成你希望的名字. 比如在我这个slides中, 名字为 slides-maker
- 上传到github中, 构建一个repo即可. 
    - 这里需要注意的是, 构建repo,运行过一次workflow之后, 需要在Settings中选择Pages, 将source修改成gh_pages.这下就可以在xxx.github.io/slides-maker/(这里的名字和上面你在`pakage.json`里修改的name保持相同)上看到你做的ppt啦. 


## 可以选择的主题
[这里](https://cn.sli.dev/themes/gallery.html)有很多可以选择的主题, 当然你也可以适用本模板的主题, 是根据[Penguin](https://github.com/alvarosabu/slidev-theme-penguin)修改而来. 特别地, 修改了加入表明author的footnote.

## 如何用markdown来写ppt
参考Slidev项目的[文档](https://cn.sli.dev/guide/)