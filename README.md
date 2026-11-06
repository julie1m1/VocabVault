# Word Vault — 单词发音本

截图导入单词与句子，自动 OCR 识别、翻译、发音。

## 功能

- **图片导入**：拖拽 / 粘贴 Ctrl+V / 点击选择，支持多张图片
- **OCR 识别**：基于 Tesseract.js，支持 English 和中英混合
- **手动输入**：粘贴单词或句子，每行一个，自动区分类型
- **自动翻译**：英文自动翻译为中文
- **自动音标**：单词自动获取音标显示
- **发音播放**：单词支持美式 / 英式发音，句子支持 TTS
- **搜索**：实时过滤单词或句子，搜索整个词库
- **历史记录**：按天查看学过的单词和句子；没有记录的天也显示日期
- **导出**：一键导出为 txt 文件
- **主题切换**：深色 / 浅色主题
- **数据持久化**：所有数据存储在 IndexedDB；首次打开自动迁移旧 localStorage 数据

## 使用方法

1. 直接在浏览器中打开 `index.html`
2. 通过截图粘贴或拖拽图片导入单词
3. 也可在文本框中手动输入单词或句子
4. 点击「添加到词库」即可
5. 点顶栏「历史」按天回看；主页最多显示今天全部 + 补足到 50 条，更多记录在历史页

## 技术栈

- 纯 HTML / CSS / JavaScript，无构建依赖
- [IndexedDB](https://developer.mozilla.org/docs/Web/API/IndexedDB_API) — 本地词库与按天历史记录
- [Tesseract.js](https://github.com/naptha/tesseract.js) — OCR 文字识别
- [Google Fonts](https://fonts.google.com/) — Outfit + IBM Plex Mono 字体
- [Youdao Dictionary](https://dict.youdao.com/) — 单词发音
- [Google Translate TTS](https://translate.google.com/) — 句子发音
- [MyMemory API](https://mymemory.translated.net/) — 英中翻译
- [ECDICT](https://github.com/skywind3000/ECDICT) — 本地音标数据库（21.8万词条，无需翻墙）
- [Moby Hyphenation List](https://www.gutenberg.org/ebooks/3204) — 音节划分数据（15.2万词条，公有领域）
