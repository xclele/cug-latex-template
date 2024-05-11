<h1 align="center">
  自制CUG（中国地质大学）本科课程作业模板
</h1>

<p align="center">
  基于中山大学非官方的课程大作业模版修改
</p>


## 介绍
- 用于CUG课程大作业/结课汇报的通用简易Latex模板
- 在[中山大学模板](https://www.texpage.com/template/21db014e-5065-448c-a6f2-545b983aee2d)的基础上进行了修改

## 模板下载

* 页面右边点击：**Clone or download -> Download Zip**

## 使用方法
默认模板文件由以下四部分组成：

- `main.tex` 主文件,包含报告正文
- `reference.bib` 参考文献列表
- `SYSUReport.sty` 文档格式控制
- `figures` 放置图片的文件夹，模板中现在包含院校LOGO和效果预览图。

使用时只需要修改 `main.tex` 和 `reference.bib` 即可，论文插图可以放在 `figures` 文件夹下，模板可以自动识别常见的插图文件夹，如 `figures`、`image`、`img` 等。

**overleaf上封面姓名处使用自定义楷体可能会缺字体渲染不出来，可以考虑自己装字体或者使用TexPage。**

--------- 
**推荐使用[TexPage](https://www.texpage.com/)** 在线进行文档的编写和编译，无需进行本地安装。在不进行其他网络设置的情况下，国内访问的速度和稳定性也要比 Overleaf 好一些。

---------

|  [封面效果图](https://my.microsoftpersonalcontent.com/personal/dc3594c94313e18b/_layouts/15/download.aspx?UniqueId=1433a0c5-3681-45a2-a9bb-43127df928b8&Translate=false&tempauth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHBfZGlzcGxheW5hbWUiOiJHcmFwaCIsImFwcGlkIjoiMDAwMDAwMDMtMDAwMC0wMDAwLWMwMDAtMDAwMDAwMDAwMDAwIiwiYXVkIjoiMDAwMDAwMDMtMDAwMC0wZmYxLWNlMDAtMDAwMDAwMDAwMDAwL215Lm1pY3Jvc29mdHBlcnNvbmFsY29udGVudC5jb21AOTE4ODA0MGQtNmM2Ny00YzViLWIxMTItMzZhMzA0YjY2ZGFkIiwiY2FjaGVrZXkiOiIwaC5mfG1lbWJlcnNoaXB8MDAwM2JmZmRkNGU4ODcwMkBsaXZlLmNvbSIsImNpZCI6InFNWFBVTUNuMjB1cytibE0xaWZyb2c9PSIsImVuZHBvaW50dXJsIjoiMEluSlpCZmtBTDZtbTA4ZU4rQjZEUjhLSnV5dmF5dzM3MkJLaUgyTFBXdz0iLCJlbmRwb2ludHVybExlbmd0aCI6IjE1MyIsImV4cCI6IjE3MTU0MzUxNzgiLCJpcGFkZHIiOiI1Mi4xMDQuMTAwLjE0MSIsImlzbG9vcGJhY2siOiJUcnVlIiwiaXNzIjoiMDAwMDAwMDMtMDAwMC0wZmYxLWNlMDAtMDAwMDAwMDAwMDAwIiwibmJmIjoiMTcxNTQzMTU3OCIsInB1aWQiOiIwMDAzQkZGREQ0RTg4NzAyIiwic2NwIjoibXlmaWxlcy5yZWFkIGFsbGZpbGVzLndyaXRlIGFsbHByb2ZpbGVzLnJlYWQiLCJzaWQiOiIzOTk5MjkxODcyMzc4MDQ0NDk1XzhjODkwYmJhLWU2ZjgtNGRmOC04MTUzLWE2NjA4M2Y5ZGQ3MyIsInNpdGVpZCI6Ik56TXhNbU15WkRJdE5qTTNZaTAwTnpaaExUbG1OMkl0TlRkaVltUmhPRFUxTkRJNCIsInRpZCI6IjkxODgwNDBkLTZjNjctNGM1Yi1iMTEyLTM2YTMwNGI2NmRhZCIsInR0IjoiMiIsInVwbiI6InhjbGVsZUBvdXRsb29rLmNvbSIsInZlciI6Imhhc2hlZHByb29mdG9rZW4ifQ.vSJobEwdG8yhxECPTgldKQSUAjK-18eFjEcmDdWtNQI&ApiVersion=2.0) |  [目录效果图](https://github.com/NorthSecond/Latex_Template/blob/main/figures/index.png)| 
|:---:|:---:|
| ![](https://my.microsoftpersonalcontent.com/personal/dc3594c94313e18b/_layouts/15/download.aspx?UniqueId=1433a0c5-3681-45a2-a9bb-43127df928b8&Translate=false&tempauth=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhcHBfZGlzcGxheW5hbWUiOiJHcmFwaCIsImFwcGlkIjoiMDAwMDAwMDMtMDAwMC0wMDAwLWMwMDAtMDAwMDAwMDAwMDAwIiwiYXVkIjoiMDAwMDAwMDMtMDAwMC0wZmYxLWNlMDAtMDAwMDAwMDAwMDAwL215Lm1pY3Jvc29mdHBlcnNvbmFsY29udGVudC5jb21AOTE4ODA0MGQtNmM2Ny00YzViLWIxMTItMzZhMzA0YjY2ZGFkIiwiY2FjaGVrZXkiOiIwaC5mfG1lbWJlcnNoaXB8MDAwM2JmZmRkNGU4ODcwMkBsaXZlLmNvbSIsImNpZCI6InFNWFBVTUNuMjB1cytibE0xaWZyb2c9PSIsImVuZHBvaW50dXJsIjoiMEluSlpCZmtBTDZtbTA4ZU4rQjZEUjhLSnV5dmF5dzM3MkJLaUgyTFBXdz0iLCJlbmRwb2ludHVybExlbmd0aCI6IjE1MyIsImV4cCI6IjE3MTU0MzUxNzgiLCJpcGFkZHIiOiI1Mi4xMDQuMTAwLjE0MSIsImlzbG9vcGJhY2siOiJUcnVlIiwiaXNzIjoiMDAwMDAwMDMtMDAwMC0wZmYxLWNlMDAtMDAwMDAwMDAwMDAwIiwibmJmIjoiMTcxNTQzMTU3OCIsInB1aWQiOiIwMDAzQkZGREQ0RTg4NzAyIiwic2NwIjoibXlmaWxlcy5yZWFkIGFsbGZpbGVzLndyaXRlIGFsbHByb2ZpbGVzLnJlYWQiLCJzaWQiOiIzOTk5MjkxODcyMzc4MDQ0NDk1XzhjODkwYmJhLWU2ZjgtNGRmOC04MTUzLWE2NjA4M2Y5ZGQ3MyIsInNpdGVpZCI6Ik56TXhNbU15WkRJdE5qTTNZaTAwTnpaaExUbG1OMkl0TlRkaVltUmhPRFUxTkRJNCIsInRpZCI6IjkxODgwNDBkLTZjNjctNGM1Yi1iMTEyLTM2YTMwNGI2NmRhZCIsInR0IjoiMiIsInVwbiI6InhjbGVsZUBvdXRsb29rLmNvbSIsInZlciI6Imhhc2hlZHByb29mdG9rZW4ifQ.vSJobEwdG8yhxECPTgldKQSUAjK-18eFjEcmDdWtNQI&ApiVersion=2.0) | ![](https://github.com/NorthSecond/SYSU_Latex_Template/blob/main/figures/index.png?raw=true)| 

## 参考

+ [国科大通用课程大作业模板](https://github.com/jweihe/UCAS_Latex_Template)
+ [GBT7714-2015标准下的BibTex样式](https://github.com/zepinglee/gbt7714-bibtex-style)
+ [国科大学位论文LaTeX模板](https://github.com/mohuangrui/ucasthesis)
+ [北京大学课程论文模板](https://www.overleaf.com/latex/templates/bei-jing-da-xue-ke-cheng-lun-wen-mo-ban/yntmqcktrzfh)
+ [中山大学课程论文模板](https://www.texpage.com/template/21db014e-5065-448c-a6f2-545b983aee2d)
