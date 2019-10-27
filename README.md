# 一个简洁优雅的 XeLaTeX 简历模板

Hit branch [master](https://github.com/billryan/resume/tree/master) if you wanna an English résumé.

每年的9月10月是求职的高峰季，除了简历上充实的干货之外，一份美美的简历自然是能助你一臂之力的啦。

\LaTeX 的简历模板其实是有不少的，坊间流传较广的有 `moderncv`, 这货使用起来比较简单，样式改起来也很方便，但是不太适合作为一页纸简历模板，因为空白太多了。传统的 `resume` 宏包虽然适合用作一页纸简历，但是定制起来比较麻烦，需要懂不少 \TeX 语法。看过不少模板，老是觉得有什么地方不满意(处女座改变世界...)，思来想去俺就自己从 ShareLaTeX 网站上找了个极简教程自己鼓捣了一个还算优雅的简历模板出来。

受以下项目启发：

- [zachscrivena/simple-resume-cv](https://github.com/zachscrivena/simple-resume-cv)
- [res](https://www.ctan.org/pkg/res)
- [JianXu's CV](http://www.jianxu.net/en/files/JianXu_CV.pdf)
- [Web Front-End Wenli Zhang.pdf](http://zhangwenli.com/cv/Web%20Front-End%20Wenli%20Zhang.pdf)
- [paciorek's CV/Resume template](http://www.stat.berkeley.edu/~paciorek/computingTips/Latex_template_creating_CV_.html)
- [How to write a LaTeX class file and design your own CV (Part 1) - ShareLaTeX](https://www.sharelatex.com/blog/2011/03/27/how-to-write-a-latex-class-file-and-design-your-own-cv.html)

其中最后一条 shareLaTeX 的总结清晰易懂，强烈建议围观。接下来介绍模板使用细节和定制说明。

## 简介

该简历模板使用 \XeLaTeX 编译，无痛支持中文，开箱即用(几乎不需要懂 \LaTeX 语法)，除了本地编译外也可使用 Sharelatex **在线编译**，无需在本机安装 TeX 发行版。

主要的功能如下：

- 极其容易定制和扩展。
- 完善的 Unicode 字体支持，因为用的是 XeLaTeX 嘛
- 完美的简体中文支持，默认使用 adobefonts 的四套简体中文字型，其他字型可自行添加。
- 支持图标字体 FontAwesome 4.6.3

### 样例输出

![English](https://user-images.githubusercontent.com/1292567/62409353-3fecfc00-b608-11e9-8e83-84962912c956.png)
![English with photo](https://user-images.githubusercontent.com/1292567/62409351-3f546580-b608-11e9-9f6d-d232a68c5451.png)
![简体中文](https://user-images.githubusercontent.com/1292567/62409352-3fecfc00-b608-11e9-8d9e-76243ca3052a.png)

- [英文 PDF](https://github.com/billryan/resume/files/3463503/resume.pdf)
- [加入照片的英文 PDF](https://github.com/billryan/resume/files/3463501/resume_photo.pdf)
- [简体中文 PDF](https://github.com/billryan/resume/files/3463502/resume-zh_CN.pdf)

## 使用方法

### ShareLaTeX 在线编译

感谢万能的『云计算』，\LaTeX 编译也可以放到云端了！使用这种方法无需在本机安装诸如 CTeX/TeXlive/MacTeX 等发行版，网站上还能有历史版本记录，十分方便！最简单的方法，浏览器中打开 [模板链接](https://www.sharelatex.com/templates/556b27cf0d23e5a8117053d9), 按需更改自己的名字和联系方式等。
在线预览时需要注意 ShareLaTeX 自带的 PDF 阅读器对中文支持不太好(可能会显示乱码)，这时在编辑界面的左侧菜单选择使用 native 阅读器即可。

中文模板的文件为 `resume-zh_CN.tex`, 英文模板的文件为 `resume.tex`, 带照片的模板文件为 `resume_photo.tex`.

### latexonline.cc

使用 [LaTeX.Online](https://latexonline.cc/) 在线编译

### 使用较新的 TeX 发行版在本地计算机编译

除了在线编译外，该模板当然也支持传统的本地编译，从 <https://github.com/billryan/resume/tree/zh_CN> 上克隆下来使用 XeLaTeX 编译即可。


```
xelatex resume.tex % 编译英文简历
xelatex resume_photo.tex % 编译带照片的简历
xelatex resume-zh_CN.tex % 编译中文简历
```

### 中英文双语支持


