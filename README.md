# CWA Weather Frontend - 看天望氣

一個美觀的台灣天氣預報前端應用，使用動森風格設計，串接本地 CWA 天氣預報 API 服務。

## 功能特色

- 🎨 動森風格的可愛界面設計
- 🌍 支援台灣 22 個縣市天氣查詢
- 📱 響應式設計，適配各種螢幕尺寸
- 🎯 直觀的城市選擇器
- 📊 清晰的天氣資訊展示
  - 當前時段天氣
  - 溫度顯示
  - 降雨機率
  - 穿搭建議
  - 36小時預報

## 使用方式

### 前置需求

1. 確保後端服務已啟動並運行在 `http://localhost:2000`
2. 後端需要有效的 CWA API Key（請參考後端專案的 README）

### 啟動應用

#### 方法一：直接開啟 HTML

直接用瀏覽器開啟 `index.html` 檔案即可使用。

#### 方法二：使用本地伺服器（推薦）

使用 VS Code 的 Live Server 擴充套件，或者使用任何本地伺服器：

```bash
# 使用 Python 3
python -m http.server 8000

# 使用 Node.js http-server
npx http-server -p 8000
```

然後在瀏覽器開啟 `http://localhost:8000`

## 專案結構

```
CwaWeather-frontend/
├── index.html          # 主要 HTML 檔案（包含 CSS 和 JavaScript）
├── icon-v2.png         # 應用圖示
├── CNAME               # GitHub Pages 設定
└── README.md          # 說明文件
```

## 使用說明

1. **選擇城市**：點擊左上角的城市選擇器，從下拉選單選擇想查詢的縣市
2. **查看當前天氣**：主卡片顯示當前時段的天氣狀況、溫度、降雨機率和衣著建議
3. **查看未來預報**：橫向滑動查看接下來的天氣預報

## 技術特點

- **純前端實現**：使用原生 HTML、CSS、JavaScript
- **零依賴**：無需安裝任何 npm 套件
- **美觀設計**：
  - 使用 Zen Maru Gothic 字體
  - 柔和的色彩配置
  - 流暢的動畫效果
  - 動森風格的 UI 元素

## 支援的城市

臺北市、新北市、桃園市、臺中市、臺南市、高雄市、基隆市、新竹市、嘉義市、新竹縣、苗栗縣、彰化縣、南投縣、雲林縣、嘉義縣、屏東縣、宜蘭縣、花蓮縣、臺東縣、澎湖縣、金門縣、連江縣

## API 連接設定

前端預設連接到 `http://localhost:2000/api/weather`。如需修改，請編輯 `index.html` 中的：

```javascript
const API_BASE_URL = "http://localhost:2000/api/weather";
```

## 注意事項

1. 確保後端服務在 `http://localhost:2000` 正常運行
2. 如果遇到 CORS 問題，請確認後端已正確設定 CORS
3. 建議使用現代瀏覽器（Chrome、Firefox、Safari、Edge）以獲得最佳體驗

## 開發者資訊

- 設計風格：動物森友會（Animal Crossing）
- 字體：Zen Maru Gothic
- 色彩方案：柔和的綠色和奶油色調

## 授權

MIT
