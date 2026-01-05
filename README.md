Omplexity Email Builder | 專業電子郵件生成器
Omplexity Email Builder 是一個專為 Omplexity 團隊設計的內部工具，旨在快速生成符合品牌視覺規範（CI）的 HTML 電子郵件。透過模組化的設計，使用者無需撰寫複雜的 HTML/CSS 程式碼，即可組合出精美的課程通知、招募信件或商務邀請函。

🚀 主要功能
品牌一致性：內建 Omplexity 品牌色系（Violet, Gold）與標準字體。

模組化設計：可自由搭配 Header、Body 與 Footer。

即時預覽：所見即所得，右側即時顯示渲染結果。

HTML 原始碼匯出：一鍵生成 HTML，可直接貼入 Gmail/Outlook。

LLM 輔助：內建 AI Prompt 指引，協助生成 HTML 內文。

💻 環境建置與使用教學 (Step-by-Step)
如果是第一次使用此工具，請按照以下步驟完成電腦設定。

步驟 1：下載並安裝 Python (底層環境)
此工具是基於 Python 語言撰寫，電腦必須先安裝 Python 才能運作。

前往 Python 官網下載頁面：Download Python。

下載最新版本的 Python (建議 3.10 以上)。

⚠️ 重要： 在安裝視窗中，務必勾選底部的 "Add Python to PATH" (將 Python 加入環境變數)，然後點擊 "Install Now"。

如果沒勾選此選項，後續的終端機指令將無法運作。

步驟 2：安裝 VS Code (建議編輯器)
雖然可以用任何文字編輯器，但推薦使用 VS Code 來執行與編輯。

前往 VS Code 官網 下載並安裝。

安裝完成後，打開 VS Code。

點擊左上角 File -> Open File...，選擇你的程式檔案 (例如桌面的 Email 2.py)。

步驟 3：安裝 Streamlit 套件
Python 安裝好後，需要安裝這個工具依賴的 streamlit 庫。

在電腦中搜尋並打開 「命令提示字元」 (Command Prompt / cmd)，或是直接在 VS Code 上方選單點選 Terminal -> New Terminal。

在黑色視窗中輸入以下指令並按 Enter：

Bash

pip install streamlit
等待跑出 Successfully installed... 字樣即代表安裝完成。

步驟 4：啟動程式
每次要使用工具時，請執行此步驟。

打開 VS Code 的終端機 (Terminal)。

複製並貼上以下指令 (路徑請依照實際檔案位置)：

Bash

streamlit run "c:/Users/Boris Wu/Desktop/Email 2.py"
(註：若檔案不在 Boris 的桌面上，請將路徑修改為檔案實際存放的位置)

按下 Enter 後，系統會自動開啟瀏覽器，你就會看到 Email Builder 的操作介面了！

📖 操作指南
介面分為左右兩欄：

1. 結構設定 (左側)
Header / Footer：選擇適合的信件抬頭與結尾樣式。

內容編輯：

載入模板：透過下拉選單載入「實體班通知」、「結訓信」等預設文案。

編輯內文：直接修改框內文字，支援 HTML 標籤 (如 <br> 換行)。

行動呼籲：勾選後可加入自定義按鈕。

2. 預覽與輸出 (右側)
確認右側預覽畫面無誤。

複製下方的 HTML 原始碼。

將原始碼貼入 Gmail (需透過 Insert HTML 工具) 或 Outlook 使用。

⚙️ 開發者指南 (如何修改內容)
若需永久修改模板內容（例如更改地址或標準文案），請直接編輯 .py 檔案：

修改顏色：搜尋 BRAND_COLORS 字典。

新增 Header：搜尋 HEADERS 字典並加入新 HTML。

修改預設文案：搜尋 BODY_TEMPLATES 字典。

License
© 2026 Omplexity. All rights reserved. Internal Tool.
