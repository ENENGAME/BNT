# **如何將檔案上傳到 GitHub**

這份教學將詳細說明如何將檔案上傳到 GitHub，適合新手快速上手。

---

## **操作步驟**

### **步驟 1：創建 GitHub 儲存庫**

1. 登入 [GitHub](https://github.com/) 帳號。
2. 點擊右上角的 `+`，選擇 **New Repository**。
3. 填寫以下資訊：
   - **Repository Name**：輸入儲存庫名稱，例如 `MyFirstRepo`。
   - **Description**（可選）：描述儲存庫用途。
   - **Visibility**：選擇 Public 或 Private。
4. 點擊 **Create Repository** 按鈕完成創建。

![創建儲存庫](https://via.placeholder.com/800x400.png?text=GitHub+Create+Repository)
*圖 1：創建新的儲存庫*

---

### **步驟 2：克隆儲存庫到本地端**

1. 在儲存庫主頁，點擊 **Code** 按鈕。
2. 複製 HTTPS 或 SSH 連結。
3. 開啟終端機（Terminal 或 CMD），執行以下指令：

   ```bash
   git clone <儲存庫網址>
   ```

4. 成功後，本地會出現一個與儲存庫同名的資料夾。

範例：
```bash
git clone https://github.com/YourUsername/MyFirstRepo.git
```

![克隆儲存庫](https://via.placeholder.com/800x400.png?text=Git+Clone)
*圖 2：克隆儲存庫到本地端*

---

### **步驟 3：新增檔案到儲存庫**

1. 將檔案複製到剛剛克隆的資料夾中。
2. 在終端機中進入該資料夾：

   ```bash
   cd MyFirstRepo
   ```

3. 使用 `git status` 檢查檔案變更狀態：

   ```bash
   git status
   ```

![新增檔案](https://via.placeholder.com/800x400.png?text=Git+Add+File)
*圖 3：新增檔案後檢查狀態*

---

### **步驟 4：提交與推送變更**

1. 將檔案加入版本控制：

   ```bash
   git add .
   ```

2. 提交變更並添加描述：

   ```bash
   git commit -m "新增檔案範例"
   ```

3. 推送到 GitHub 儲存庫：

   ```bash
   git push origin main
   ```

4. 成功後，可以在 GitHub 網頁檢視上傳的檔案。

![推送變更](https://via.placeholder.com/800x400.png?text=Git+Push)
*圖 4：推送檔案到遠端儲存庫*

---

## **常見問題**

1. **為什麼推送失敗？**
   - 確保已經使用 `git config` 設置使用者名稱與信箱。
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "youremail@example.com"
   ```

2. **如何同步遠端儲存庫更新？**
   - 使用以下指令更新本地儲存庫：
   ```bash
   git pull origin main
   ```

---

完成以上步驟後，您已成功將檔案上傳至 GitHub！
