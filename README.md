# gen-markdown-content
    功能：自动生成markdown文件的目录，便于大文件导航。

    用法：`python gmc.py srcFileName.md`即可在当前目录下生成名为res.md的带有目录的md文件。

    原理：采用md和html混编，利用`[name](#hid)`和`<h1 id=hid>name</h1>`实现跳转。

提示：    
    * 目录样式可以在代码中自行修改。
    * 浏览markdown渲染后的文件时可随时按`home`键回到文件头部，再根据目录任意跳转。
    * 使用效果良好的前提是标题书写规范，即满足正则匹配`'#+\s'`,当然，也可以修改正则。   

效果展示： 
[样例文章](http://www.cnblogs.com/findneo/p/7083078.html)
![sample.png](https://ooo.0o0.ooo/2017/06/27/595222c8d1b5f.png)
