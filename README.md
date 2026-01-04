## 安裝
### Windows

1. 到 Node.js 官網 下載 LTS 版本的Node.js，並打開 PowerShell 或命令提示字元執行以下指令驗證安裝
    ```
    node -v
    npm -v
    ```
2. 透過安裝 n8n CLI ，並打開 PowerShell 或命令提示字元驗證安裝
    ```
    npm install -g n8n
    n8n --version
    ```

## 快速開始

在 PowerShell 或命令提示字元執行以下指令啟動 n8n：

```powershell
n8n start
```

在瀏覽器開啟 `http://localhost:5678` 即可開始使用 n8n 建立工作流


## Github 工作流資料同步

### 上傳
1. 在 PowerShell 或命令提示字元輸入以下指令，將所有工作流匯出至`workflows`資料夾
   ```
   n8n export:workflow --all --output=workflows/
   ```
2. 於 Github Desktop 點擊提交並推送專案

### 下載同步
1. 於 Github Desktop 拉取最新變更
2. 在 PowerShell 或命令提示字元輸入以下指令，將`workflows`資料夾中的工作流匯入至 n8n
   ```
   n8n import:workflow --input=workflows/
   ```
