# DIY_MX
## 起因
前段时间在网上找毛选的PDF版本，结果没有找到合适的，要么由于字体原因打开后是乱码，要么版本自己不喜欢（有人搜集制作了一个1-5卷的合集，我不是很喜欢，尤其是制作者加上了个人信息，看着很别扭）。 所以自己决定弄一个。
## 方法（爬虫+LaTeX）
### 爬虫
自己第一次用Python写爬虫，写的真的很垃圾（大神莫笑话），不过还是生成了大部分latex code。爬的是[这个网站](https://www.marxists.org/chinese/maozedong/index.htm)
### LaTeX
latex模板我使用的是[ElegantBook](https://www.overleaf.com/latex/templates/elegantbook-template/zpsrbmdsxrgy)，由于我喜欢用overleaf，就在上面找了该模板，并做了一点点的修改。
## 具体过程
1. MX_V1.ipynb 生成卷一所需的latex， MX_V2345.ipynb 生成卷二三四五所需的latex。（每次生成一卷，保存在2.txt中。 再次强调代码是胡乱写的，太垃圾了。）
2. LaTeX code拷贝到相应的.tex文件中，自己再手动更改一下封面等（每一卷一本书）。 这里说一下Python代码只生成了该卷中每篇文章对应的LaTeX代码，其他的部分请看MX.tex文件。
## 结果
1. 做了卷一至五（保存在PDF文件夹中，由于我不喜欢给目录中文章加上数字编号，所以在LaTeX中用了Section* 而不是 Section，导致PDF中点击左侧相应的文章名字是没有反应的）
2. 未删节版本也附在正式文章之后
3. 卷一附了《辩证法唯物论（讲授提纲）》（* 内含《实践论》与《矛盾论》的原始版本）
4. 卷五附了网站中**其他**里的六篇
5. 封面选了让子弹飞里的九筒，太祖头像，和相应卷里的一句话
6. 自己不喜欢注释放在文章最后的方式（翻来倒去太麻烦），于是就把注释放在该页最下了。
## 后续工作
目前只过了一遍卷一，改了一些错误（爬虫code是不好改了，加了太多的if-elif-else，自己已经晕了，只好在latex直接改）。 卷二三四五还没仔细看，但也改了一些过于明显的错误。后续会继续更新LaTeX，大家如果发现可以直接commit或者发邮件给[我](mailto:ningzhang0123@gmail.com)。
## 版权
版权应该还属于太祖吧，如果有懂法律的哥们儿发现我这属于侵权，请通知我，我立马删除。不过我觉得带头大哥应该不在乎这些，他写这些本来就是让大家看的。所以我也无所谓，请大家随意下载，传播，更改。。。

