# BDSE end of term project

本專案使用 Docker Compose 建立一個可協作的多容器環境，其中為處理 City 數據匯入、儲存、網頁呈現，建立以下四個容器：

1. MySQL 資料庫容器
2. ETL 資料處理容器（匯入 city_feature.csv）
3. Web 容器（Flask 顯示 HTML 頁面）
4. Streamlit 容器（資料視覺化城市指標）

請見下方啟動方式與任務分工。

## 環境需求

- Docker & Docker Compose
- git

## 啟動方式

```bash
git clone https://github.com/JackLaiplus/Project-BDSE-end-of-term-project.git
cd Project-BDSE-end-of-term-project
docker compose up -d --build # 在背景執行
```

## 專案結構簡介

|目錄 | 用途 |
|---------------|------|
| init/         | 初始 SQL 建表檔 |
| city_mysql/   | MySQL 資料庫容器 |
| city_loader/   | ETL 資料處理容器 |
| city_web/          | Flask 顯示 HTML 頁面 |
| city_streamlit/    | 資料視覺化城市指標 |
