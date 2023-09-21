# PDF英文转中文

生成的PDF是中英对照的。

<p align="center">
  <img src="./assets/sample1.png" width=100%>
</p>

## 概述

Thanks to [PDF Translator EN-JA](https://github.com/discus0434/pdf-translator)

为了方便看英文文献，在网上找了一些PDF翻译器，最后Fork上面的仓库，做了点修改。

需要配置本地运行环境，运行main.py即可，需要下载模型到本地。使用paddleOCR提取文本，使用[hugging face模型](https://huggingface.co/Helsinki-NLP/opus-mt-en-zh)进行中英文翻译。完全离线。

# 使用方法：

按顺序执行以下操作（仅在windows11 x64进行了使用操作，不保证支持其他平台）：
0. 确保控制台cmd或powershell可以运行python，并具有git，cd到你常用的工作目录下
1. git clone https://github.com/babakara/pdf-translator
2. cd pdf-translator
3. python -m venv venv
4. pip install -r requirements.txt
5. python main.py

# 补充说明
如果要更换示例的PDF文件，替换"translate_pdf/123.pdf"。
生成的中间文件在"temp"文件夹下
合并结果PDF在"outputs\translated.pdf"