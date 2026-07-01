# Word Vault — 单词发音本

截图导入单词与句子，自动 OCR 识别、翻译、发音。

## 功能

- **图片导入**：拖拽 / 粘贴 Ctrl+V / 点击选择，支持多张图片
- **OCR 识别**：基于 Tesseract.js，支持 English 和中英混合
- **手动输入**：粘贴单词或句子，每行一个，自动区分类型
- **自动翻译**：英文自动翻译为中文
- **自动音标**：单词自动获取音标显示
- **发音播放**：单词支持美式 / 英式发音，句子支持 TTS
- **搜索**：实时过滤单词或句子
- **导出**：一键导出为 txt 文件
- **主题切换**：深色 / 浅色主题
- **数据持久化**：所有数据存储在 localStorage

## 使用方法

1. 直接在浏览器中打开 `Tool-生词 自动转换声音和意思音标.html`
2. 通过截图粘贴或拖拽图片导入单词
3. 也可在文本框中手动输入单词或句子
4. 点击「添加到词库」即可

## 技术栈

- 纯 HTML / CSS / JavaScript，无构建依赖
- [Tesseract.js](https://github.com/naptha/tesseract.js) — OCR 文字识别
- [Google Fonts](https://fonts.google.com/) — Outfit + IBM Plex Mono 字体
- [Youdao Dictionary](https://dict.youdao.com/) — 单词发音
- [Google Translate TTS](https://translate.google.com/) — 句子发音
- [MyMemory API](https://mymemory.translated.net/) — 英中翻译
- [DictionaryAPI](https://dictionaryapi.dev/) — 英文音标
