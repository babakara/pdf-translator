# PDF Translator EN-ZH

生成的PDF是中英对照的。

<p align="center">
  <img src="./assets/sample1.png" width=100%>
</p>

## Features

Thanks to [PDF Translator EN-JA](https://github.com/discus0434/pdf-translator)

为了方便看英文文献，在网上找了一些PDF翻译器，最后Fork上面的仓库，做了点修改。

# 使用方法：

按顺序执行以下操作（仅在windows11 x64进行了使用操作，不保证支持其他平台）：
0. 确保控制台cmd或powershell可以运行python，并具有git，cd到你常用的工作目录下
1. git clone https://github.com/babakara/pdf-translator
2. cd pdf-translator
3. python -m venv venv
4. pip install -r requirements.txt
5. python main.py

如果要更换示例的PDF文件，替换"translate_pdf/123.pdf"。
生成的中间文件在"temp"文件夹下
合并结果PDF在"outputs\translated.pdf"