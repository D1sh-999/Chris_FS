# 女装选品小站 部署包

## 上传最重要一点
把 data 整个文件夹一起传,CSV 要在 data/products.csv。
(即使不小心传到根目录,本版本也会自动回退到根目录的 products.csv,但仍建议放 data 里)

## 目录结构
index.html / config.js / data/products.csv

## 部署(GitHub Pages)
1. 仓库根目录上传 index.html、config.js、整个 data 文件夹。
2. Settings -> Pages -> Source 选 main / (root),保存。
3. 等 1~2 分钟访问 https://<用户名>.github.io/<仓库名>/ 。

## 口令
config.js 只存 SHA-256 哈希,无明文。改口令需重算哈希替换 accessCodeHash / adminCodeHash。

## 更新货盘
- 临时:管理员口令进站 -> 货盘管理 -> 上传 CSV/Excel(仅当前浏览器)。
- 永久:替换 data/products.csv 重新提交。
