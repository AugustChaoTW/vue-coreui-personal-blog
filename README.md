# vue-coreui-personal-blog
基於 Vue.js 和 CoreUI 框架的個人部落格專案

## 專案結構

### 頁面組件

#### Welcome.vue
位置：`src/views/Welcome.vue`

歡迎頁面組件，使用 Vue 3 與 CoreUI 元件建置。此頁面作為網站的歡迎首頁，展示 "Welcome to Aug's Home!" 訊息。

**功能特色：**
- 使用 CoreUI 的卡片組件 (CCard) 建構主要內容區域
- 包含漸層背景設計，提供優雅的視覺效果
- 響應式設計，適配不同螢幕尺寸
- 整合 CoreUI 圖示系統

**使用的 CoreUI 組件：**
- CContainer: 容器組件
- CRow/CCol: 響應式網格系統
- CCard/CCardHeader/CCardBody: 卡片組件
- CIcon: 圖示組件
