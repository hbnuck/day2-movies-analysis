# 🎬 Day 2：簡易電影推薦系統實作

本專案透過 `genre`, `score`, `votes`, `gross` 等特徵，建構簡易電影推薦引擎，目標為輸入一部電影名稱，推薦前 5 名相似電影。

---

## 📌 使用資料
- 資料集：movies.csv（IMDB 資料延伸）
- 欄位包含：電影名稱、評分（score）、票房（gross）、投票數（votes）、類型（genre）

---

## 🔧 使用技術
- `pandas` 做資料處理與特徵矩陣建立
- `get_dummies()` 將 genre 做 one-hot encoding
- `cosine_similarity()` 比較電影特徵相似度
- `sort_values()` 排出最相似 Top-N

---

## 🧪 推薦範例
```python
recommend("Inception")
