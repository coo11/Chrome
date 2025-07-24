# Import Custom Search Engines

## Chrome

自 Chrome 137 以来，存储搜索引擎数据的文件[添加了数据验证](https://chromium.googlesource.com/chromium/src.git/+/refs/tags/137.0.7151.138/components/search_engines/keyword_table.h#88)，因此原本通过数据库导入搜索引擎的方法失效。现在的方法是在 `chrome://settings/searchEngines` 页面，将本目录下 `engines.json` 中的数据和 `importEngines.js` 中的代码在开发者工具中执行来导入。

[查看拼接好的 importEngines.js](https://raw.githubusercontent.com/coo11/Chrome/refs/heads/output/importEngines.js)