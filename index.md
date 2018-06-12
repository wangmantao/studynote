# 学习笔记
## 工作效率类
### emacs 实现代码PDF转换
- steps
	需要部分（下载依赖软件）：
	1, gs软件 (有linux / windows 可选）
		https://ghostscript.com/download/gsdnld.html	
	2, Emacs配置文件 ps2pdf.el（可以让Eamcs执行用gs转换code buffer成PDF）
		https://www.emacswiki.org/emacs/ps2pdf.el

	修改配置部分：
	1. Emacs配置文件1 init.el 添加
		(load-file "c:/soft/emacs/.emacs.d/ps2pdf.el")
	2. Emacs配置文件2 ps2pdf.el
		（可执行文件gs -> gswin32.exe)
	3. windows 添加gs软件的环境变量（bin和lib目录）

	用法：
	M+x ps2pdf-buffer

	问题：
	中文字体 PDF 显示不了
### 本地新建的项目 上传到GITHUB
1. 虽然本地有新项目，github上还是要有一个仓库(它的地址以git结尾）
	仓库建好后：
		用以下命令
 
 - 在本地推一个新项目
 echo "# gitTest" >> README.md
 git init
 git add README.md
 git commit -m "first commit"
 git remote add origin https://github.com/wangmantao/gitTest.git
 git push -u origin master

- 推一个本地已有的项目
  git remote add origin https://github.com/wangmantao/gitTest.git
  git push -u origin master

