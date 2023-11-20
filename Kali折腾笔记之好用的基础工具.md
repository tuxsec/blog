首先是ssh工具，折腾云服务器的时候发现手机网用来连接服务器比我的宽带稳定，一番查找后发现了一个叫做termius的手机端工具，后来发现linux的命令行ssh不太方便，便用了termius的linux版。

ssh工具之termius:

推荐理由：操作简便，功能丰富，颜值在软件界也是很好看的。最重要的它贼稳定，比不倒翁都稳，手机上操作ssh从移动数据网到wifi的各种切换，它还是很稳定，甚至挂上代理它都还坚挺。还有不同设备同步功能也很不错。

termius Linux版：

![图片](https://github.com/tuxsec/blog/assets/26221848/5d5b261a-5b57-4237-9cbf-43afae2deb1d)


termiu Android版：

![图片](https://github.com/tuxsec/blog/assets/26221848/c1c6302a-e010-4a05-bd9d-a6975e23ae91)


其他系统也能用，功能都很全。



然后就是支持Markdown的笔记工具，在找考试用的笔记工具时候，有了几个需求：1，支持Markdown；2，可以快速把截图粘贴进去，并且它还自动生成Markdown的格式；最后找到Typora工具。推荐他的理由完全就是第二个需求，在写渗透测试报告或着考试报告的时候需要大量截图粘贴操作，并且考试模板和笔记用Markdown格式更方便复制或者发表成blog，便有了这个需求。

Typora:

![图片](https://github.com/tuxsec/blog/assets/26221848/b07b974b-a670-49ab-8376-e55e9e1f0028)


然后就是附带一个md转pdf工具，这是个命令行工具。pandoc，它可以把上面保存的.md文件转换成pdf，效果很好，这是在找考试报告模板的时候找到的，链接如下https://github.com/noraj/OSCP-Exam-Report-Template-Markdown/blob/master/src/OSED-exam-report-template_epi_v1.md ，链接里面也有自动生成考试报告的脚本，pandoc从模板到pdf的使用方法如下：

    #!/bin/bash
    pandoc ./OSED-exam-report.md \
    -o ./OSED-OS-xxxx-Exam-Report.pdf \
    --from markdown+yaml_metadata_block+raw_html \
    --template eisvogel \
    --table-of-contents \
    --toc-depth 6 \
    --number-sections \
    --top-level-division=chapter \
    --highlight-style breezedark \
    --resource-path=.:src

打包成bash脚本的pandoc：

![图片](https://github.com/tuxsec/blog/assets/26221848/ed832777-6035-45a2-a181-f379c2a631db)



截图工具，Flameshot，截图后按Ctrl + c可以把截图复制到剪贴板，按Ctrl+s可以保存到文件，保存的文件名格式也是可以编辑的，缺点是只能按照时间格式编辑。可以在截图上面绘图，还能上传到云上面。由于不能截图截图软件所以就不放截图界面的截图了（doge）。

Flameshot:

![图片](https://github.com/tuxsec/blog/assets/26221848/f6b9a297-58b9-4007-be41-dc48e11f2df9)


快捷键功能一览：

![图片](https://github.com/tuxsec/blog/assets/26221848/b09203f6-10d2-46cf-809f-3147ef77de19)



剪贴板工具，Clipman，它有个方便的功能是可以把剪贴板的内容转换成二维码，这样手机扫一下码就能快速复制内容了。它是kali自带的工具。

Clipman：


![图片](https://github.com/tuxsec/blog/assets/26221848/4f3d88cc-f698-475a-9482-dfbc52a56eb5)




因为主要是用来考试准备的，平时用也很不错。



本文禁止转载或摘编
