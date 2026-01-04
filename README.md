## Installation
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
## Github 資料同步

### 上傳
1. 在 PowerShell 或命令提示字元輸入以下指令，將所有工作流匯出至`workflows`資料夾
```
n8n export:workflow --all --output=workflows/
```
2. 於Github Desktop點擊提交並推送專案
3. 
### 上傳
