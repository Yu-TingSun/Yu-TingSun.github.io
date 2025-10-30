---
title: 'Building Your Academic Website | Hugo Academic 建站指南'
subtitle: 'A Complete Guide | 完整教程'
summary: 'Hugo Academic + Netlify deployment guide based on real experience | 基於真實經驗的建站完整指南'
authors: [admin]
tags: [Hugo, Tutorial, Web Development, Academic]
categories: [Resources]
date: 2025-10-30
featured: true
draft: false
---

<div style="background: #f0f7ff; padding: 1rem; border-radius: 8px; margin-bottom: 2rem;">

📖 **Language / 語言**

[English Version](#english-version) | [中文版本](#chinese-version)

</div>

---

# English Version {#english-version}

## Building Your Academic Website: A Complete Guide

### 🎓 About This Guide
As a researcher seeking academic positions, I needed a professional website to showcase my research accomplishments. This guide documents my complete journey of building this website using Hugo Academic (Hugo Blox) with the assistance of Claude AI (Anthropic).

**This is a real story** - someone with limited website experience successfully building a professional academic website.


### :book:  Why This Guide?

After spending considerable time exploring different approaches, I want to share:
- **Essential AI tips** - How to effectively use AI assistants and what to do when stuck
- **Key decisions that save time**
- **Common pitfalls to avoid**
- **Practical solutions that work**
- **Backup strategies that prevent data loss**

### 💡 AI Can Help You Build This

Modern AI assistants like Claude, ChatGPT, and others can help you solve virtually any technical problem you encounter. 

🔧 **Pro Tip: When AI Gets Stuck**

If you find the AI going in circles,

1. **Open a new conversation window**
2. **Organize your problem clearly:**
   - What you're trying to achieve
   - What you've tried
   - Error messages you're seeing
   - Links to previous conversations
3. **Give the AI the big picture** - Let it approach the problem from a fresh, holistic perspective

This "reset and reorganize" strategy often breaks through technical bottlenecks. **It worked when I met persistent GitHub Actions deployment failures.**



---

### Table of Contents

1. [Understanding Hugo Academic](#en-understanding)
2. [Deployment Platform: Why Netlify](#en-platform)
3. [Step-by-Step Setup](#en-setup)
4. [Common Issues & Solutions](#en-issues)
5. [Critical: Backup Strategy](#en-backup) ⚠️⚠️⚠️
6. [Key Lessons Learned](#en-lessons)
7. [Success Checklist](#en-checklist)

---

### 1. Understanding Hugo Academic {#en-understanding}

Hugo Academic (now Hugo Blox) is a static site generator specifically designed for academics and researchers.

**What is a Static Site Generator?**
- Converts Markdown files → HTML websites
- No database needed
- Fast loading, easy hosting
- Perfect for academic portfolios

**Key Advantages:**
- ✅ Professional academic design
- ✅ Publication management
- ✅ CV/Resume integration
- ✅ Research project showcase
- ✅ Active community support

---

### 2. Deployment Platform: Why Netlify {#en-platform}

**The Critical Decision**

| Platform | Setup Time | Difficulty | Recommendation |
|----------|-----------|------------|----------------|
| **Netlify** | 10 minutes | ⭐ Easy | ⭐⭐⭐⭐⭐ |
| GitHub Pages | 2-8 hours | ⭐⭐⭐ Hard | ⭐⭐ |

**My Experience:**

```
Initial attempt: GitHub Pages
↓
Encountered TailwindCSS compilation errors
↓
Spent 6+ hours debugging
↓
Switched to Netlify
↓
Deployed successfully in 10 minutes ✅
```

**Understanding the Workflow:**

Both approaches require GitHub for code hosting, but differ in deployment:
```
Your Code (Local)
     ↓
GitHub Repository (Required for both)
     ↓
   ┌─────────────────┬─────────────────┐
   │                 │                 │
GitHub Pages    OR   Netlify
(Direct deploy)      (Better build system)
     ↓                     ↓
Your Website         Your Website
yourname.github.io   yourname.netlify.app
```

**Why Netlify Works Better:**
- **Same GitHub account needed** - Your code still lives on GitHub
- **Official Hugo Blox recommendation** - Tested and supported
- **Automatic dependency handling** - Solves TailwindCSS issues
- **Zero configuration needed** - Just connect and deploy
- **Free tier sufficient** - Perfect for academic sites
- **Continuous deployment** - Auto-updates when you push to GitHub

**Key Point:** You'll still use GitHub to store and manage your code. Netlify simply reads from your GitHub repository and builds your website with better tools.


---

### 3. Step-by-Step Setup {#en-setup}

#### Phase 1: Prerequisites

```bash
# Install Hugo (macOS with Homebrew)
brew install hugo

# Verify installation
hugo version  # Should be >= 0.148.0
```

#### Phase 2: Local Setup

```bash
# Clone the official template
git clone https://github.com/HugoBlox/theme-academic-cv.git my-academic-site
cd my-academic-site

# Remove template git history
rm -rf .git

# Initialize your own repository
git init
git branch -M main

# Connect to your GitHub repository
git remote add origin https://github.com/YourUsername/YourUsername.github.io.git

# First commit
git add .
git commit -m "Initial commit: Hugo Academic site"
git push -u origin main
```

#### Phase 3: Basic Configuration

Edit `config/_default/hugo.yaml`:
```yaml
title: 'Your Name, PhD'
baseURL: 'https://yourname.netlify.app/'
```

Edit `content/authors/admin/_index.md` with your information.

#### Phase 4: Deploy to Netlify

**Step 1:** Sign up at [netlify.com](https://www.netlify.com) using GitHub

**Step 2:** Import your repository

**Step 3:** Configure build settings:
- **Branch**: `main`
- **Build command**: `hugo --gc --minify`
- **Publish directory**: `public`

**Step 4:** Add environment variables:
```
HUGO_VERSION = 0.152.1
NODE_VERSION = 20
```

**Step 5:** Deploy! Your site will be live at `https://random-name.netlify.app`

**Step 6:** Customize your URL in Site Settings → Domain Management

---

### 4. Common Issues & Solutions {#en-issues}

#### Issue 1: TailwindCSS Error

**Error Message:**
```
Error: TAILWINDCSS: failed to transform
binary with name "tailwindcss" not found
```

**Solution:**
```bash
# If error occurs locally, simply ignore it
# Push to Netlify - it will work there
git push origin main

# Or install dependencies locally
npm install
```

#### Issue 2: Content Not Updating

**Cause:** Changes not pushed to GitHub

**Solution:**
```bash
git status
git add .
git commit -m "Update content"
git push origin main
# Wait 2-3 minutes for Netlify to redeploy
```

#### Issue 3: Lost Local Files

**This is preventable!** See the next section on backup strategy.

---

### 5. ⚠️ CRITICAL: Backup Strategy {#en-backup}

**This section might save you hours of frustration.**

#### The Problem

During development, you might accidentally:
- Overwrite files with `git reset --hard`
- Lose content during merge conflicts
- Delete files unintentionally

**Without backups, your content is gone.**

---

#### The Solution: Multiple Backup Layers

##### **Layer 1: Local Folder Backups** 💾

**THIS IS THE MOST IMPORTANT**❗

After every significant editing session, backup your entire project folder:
```bash
# Basic backup command (recommended)
cp -r my-academic-site my-academic-site-backup-$(date +%Y%m%d-%H%M)

# If you get "Permission denied" error, use rsync:
rsync -av --exclude='.git' my-academic-site/ my-academic-site-backup-$(date +%Y%m%d-%H%M)/
```

**Why this matters:**
- Most direct and reliable backup method
- Complete snapshot independent of Git
- Takes 10 seconds, can save hours of work
- Easy to browse and restore

**Recommended Backup Schedule:**
- ✅ After each major content addition
- ✅ Before any risky Git operations
- ✅ At the end of each editing session
- ✅ Before updating Hugo or dependencies

**Where to store backups:**
```bash
# Create a dedicated backup folder
mkdir -p ~/Desktop/website-backups

# Backup there
cp -r my-academic-site ~/Desktop/website-backups/backup-$(date +%Y%m%d-%H%M)
```

---

##### **Layer 2: Git Commits** 📦

Commit frequently:
```bash
# After editing 1-3 files
git add .
git commit -m "Update: specific description"
git push origin main
```

**Benefits:**
- Version history tracking
- Can roll back to any point
- Automatically synced to GitHub

---

##### **Layer 3: Backup Branches** 🌿

Create periodic backup branches before major changes:
```bash
# Weekly backup
git branch backup-weekly-$(date +%Y%m%d)
git push origin backup-weekly-$(date +%Y%m%d)

# Before major redesign
git branch backup-before-redesign
git push origin backup-before-redesign
```

---

##### **Layer 4: AI Conversation Archives** 🤖

**When everything else fails, AI conversations can be a lifesaver.**

If you're using AI assistance extensively:

**Create milestone snapshots:**
- When you complete a major phase (e.g., "Initial setup complete")
- Start a new conversation with: "This is a backup conversation for [date]"
- Paste your complete current working version
- **Store outside your project folder** to avoid accidental deletion

**Why this works:**
- AI chat history persists even if local files are lost
- Can reconstruct your project from conversation history
- Documents your decision-making process
- Useful reference when similar issues arise

**Pro Tip:** Don't save every small code snippet. Instead, create comprehensive milestone backups when you reach stable states.

---

#### **Backup Workflow Summary**
```bash
# === Daily Workflow ===

# 1. Start editing
cd ~/my-academic-site

# 2. Make changes to content

# 3. Test locally (optional)
hugo server -D

# 4. Local backup (PRIORITY #1 - DO NOT SKIP!)
cp -r ~/my-academic-site ~/Desktop/website-backups/backup-$(date +%Y%m%d-%H%M)

# 5. Git commit (PRIORITY #2)
git add .
git commit -m "Update: what you changed"
git push origin main

# 6. Verify deployment on Netlify

# 7. (Optional) Create backup branch before major changes
git branch backup-before-major-change
git push origin backup-before-major-change

# 8. (Milestone) Archive complete version in AI conversation if needed
```

**Remember:** Backups are cheap, recreating lost work is expensive. Local backups are your first and most reliable safety net.

---

### 6. Key Lessons Learned {#en-lessons}

**1. Follow Official Recommendations**
- Use Netlify (not GitHub Pages)
- Use official templates
- Don't over-customize initially

**2. Commit Frequently**
```bash
# After editing 1-3 files
git add . && git commit -m "description" && git push
```

**3. AI is Your Co-Pilot**
- Don't hesitate to ask for help
- Organize your questions clearly
- Start fresh conversations when stuck
- Keep chat histories as documentation

**4. Multiple Backups Are Essential**
- Local folder copies (use `cp` or `rsync`)
- Git commits
- Backup branches
- AI conversation history

**5. Content > Technology**
- 80% time: Quality content
- 20% time: Website styling

**6. Incremental Progress**
- Small steps
- Continuous validation
- Don't try to do everything at once

---

### 7. Success Checklist {#en-checklist}

**Initial Setup:**
- [ ] Hugo and Git installed
- [ ] GitHub repository created
- [ ] Template cloned and configured
- [ ] First backup created
- [ ] Deployed to Netlify
- [ ] Custom URL set

**Content Development:**
- [ ] Personal profile updated
- [ ] Research content added
- [ ] Publications listed
- [ ] CV/Resume page created
- [ ] All links tested
- [ ] Regular backups maintained

**Maintenance:**
- [ ] Backup strategy established
- [ ] AI conversation history organized
- [ ] Mobile version tested
- [ ] Peer feedback collected

---

### Conclusion

Building an academic website is an investment:
- 💼 Showcase your research
- 🌐 Establish online presence
- 📚 Organize your work
- 🤝 Network with colleagues

**Key Takeaways:**
1. **AI tools make this accessible** - You don't need to be a developer
2. **Start fresh when stuck** - New AI conversations offer new perspectives
3. **Backup religiously** - Use `cp -r` or `rsync` after every session
4. **Organize your AI chats** - They're documentation and backups
5. **Done > Perfect** - Launch and iterate

Good luck! 🚀

---

### About This Guide

**Author:** Yu-Ting Sun, PhD  
**Built with:** Claude AI (Anthropic)  
**Last Updated:** October 30, 2025

**Source Code:** [View this website's repository](https://github.com/Yu-TingSun/Yu-TingSun.github.io)

---

## Related Resources

- **Hugo Documentation:** https://gohugo.io/
- **Hugo Blox Docs:** https://docs.hugoblox.com/
- **Netlify Docs:** https://docs.netlify.com/

---

<div style="margin: 4rem 0; border-top: 3px solid #e5e7eb;"></div>

---

# 中文版本 {#chinese-version}

## Hugo Academic 建站完整指南

### 🎓 關於本指南

作為求職中的研究者，我需要一個專業網站來展示研究成果。本指南記錄了我使用 Hugo Academic (Hugo Blox) 並在 Claude AI (Anthropic) 協助下建立本網站的完整歷程。

**這是本人的故事** -- 一個編程經驗有限的人成功建立專業學術網站。

---

### 📖 為什麼寫這份指南？

在探索了多種方案後，我想分享：

- **AI 使用要點** - 如何有效使用 AI 助手以及遇到瓶頸時的應對方法
- **節省時間的關鍵決策**
- **常見的坑和避免踩坑的方法**
- **真正有效的解決方案**
- **防止資料丟失的備份策略**

---

### 💡 AI 可以幫你建站

現代 AI 助手如 Claude、ChatGPT 等，可以幫你解決幾乎任何技術問題。

🔧 **進階技巧：當 AI 鬼打牆時**

1. **新開一個對話窗口**
2. **有條理地整理你的問題：**
   - 你的目的
   - 你已經嘗試的方法
   - 你看到的錯誤訊息和困境
   - 之前相關對話的連結
3. **給 AI 完整的大局觀** - 讓它從一個全新的、更高的維度來解決問題

這個策略通常能突破技術瓶頸。**當我遇到持續的 GitHub Actions 部署失敗時，這個方法起了作用。**

---

### 目錄

1. [理解 Hugo Academic](#zh-understanding)
2. [部署平台：為何選 Netlify](#zh-platform)
3. [完整建站步驟](#zh-setup)
4. [常見問題與解決](#zh-issues)
5. [關鍵：備份策略](#zh-backup) ⚠️⚠️⚠️
6. [核心經驗教訓](#zh-lessons)
7. [成功檢查清單](#zh-checklist)

---

### 1. 理解 Hugo Academic {#zh-understanding}

Hugo Academic（現稱 Hugo Blox）是專為學術研究者設計的靜態網站生成器。

**什麼是靜態網站生成器？**
- 將 Markdown 文件 → 轉換為 HTML 網站
- 不需要資料庫
- 載入快速，容易託管
- 非常適合學術作品集

**核心優勢：**
- ✅ 專業的學術設計
- ✅ 論文管理功能
- ✅ CV/簡歷整合
- ✅ 研究專案展示
- ✅ 活躍的社群支持

---

### 2. 部署平台：為何選 Netlify {#zh-platform}

**最關鍵的決策**

| 平台 | 設置時間 | 難度 | 推薦度 |
|------|---------|------|--------|
| **Netlify** | 10分鐘 | ⭐ 簡單 | ⭐⭐⭐⭐⭐ |
| GitHub Pages | 2-8小時 | ⭐⭐⭐ 困難 | ⭐⭐ |

**我的經驗：**
```
初次嘗試：GitHub Pages
↓
遇到 TailwindCSS 編譯錯誤
↓
花費 6+ 小時調試
↓
改用 Netlify
↓
10 分鐘成功部署 ✅
```

**理解工作流程：**

兩種方式都需要 GitHub 來存放程式碼，但部署方式不同：
```
你的程式碼（本地）
     ↓
GitHub Repository（兩種方式都需要）
     ↓
   ┌─────────────────┬─────────────────┐
   │                 │                 │
GitHub Pages    或   Netlify
（直接部署）         （更好的建置系統）
     ↓                     ↓
你的網站              你的網站
yourname.github.io   yourname.netlify.app
```

**Netlify 的優勢：**
- **同樣需要 GitHub 帳號** - 你的程式碼仍然存放在 GitHub
- **Hugo Blox 官方推薦** - 經過測試和支援
- **自動處理依賴** - 解決 TailwindCSS 問題
- **零配置需求** - 只需連接即可部署
- **免費方案足夠** - 非常適合學術網站
- **持續部署** - 推送到 GitHub 時自動更新

**重點：** 你仍然使用 GitHub 來存放和管理程式碼。Netlify 只是從你的 GitHub repository 讀取資料，並用更好的工具建置你的網站。

---

### 3. 完整建站步驟 {#zh-setup}

#### 階段 1：準備工作
```bash
# 安裝 Hugo（macOS + Homebrew）
brew install hugo

# 驗證安裝
hugo version  # 應該 >= 0.148.0
```

#### 階段 2：本地設置
```bash
# Clone 官方模板
git clone https://github.com/HugoBlox/theme-academic-cv.git my-academic-site
cd my-academic-site

# 移除模板的 git 歷史
rm -rf .git

# 初始化你自己的 repository
git init
git branch -M main

# 連接到 GitHub repository
git remote add origin https://github.com/YourUsername/YourUsername.github.io.git

# 首次提交
git add .
git commit -m "Initial commit: Hugo Academic site"
git push -u origin main
```

#### 階段 3：基本配置

編輯 `config/_default/hugo.yaml`：
```yaml
title: '你的名字, PhD'
baseURL: 'https://yourname.netlify.app/'
```

編輯 `content/authors/admin/_index.md` 填入你的資訊。

#### 階段 4：部署到 Netlify

**步驟 1：** 在 [netlify.com](https://www.netlify.com) 用 GitHub 註冊

**步驟 2：** 導入你的 repository

**步驟 3：** 配置構建設定：
- **Branch**: `main`
- **Build command**: `hugo --gc --minify`
- **Publish directory**: `public`

**步驟 4：** 添加環境變數：
```
HUGO_VERSION = 0.152.1
NODE_VERSION = 20
```

**步驟 5：** 部署！網站會上線到 `https://random-name.netlify.app`

**步驟 6：** 在 Site Settings → Domain Management 自訂網址

---

### 4. 常見問題與解決 {#zh-issues}

#### 問題 1：TailwindCSS 錯誤

**錯誤訊息：**
```
Error: TAILWINDCSS: failed to transform
binary with name "tailwindcss" not found
```

**解決方案：**
```bash
# 如果本地出現此錯誤，直接忽略
# 推送到 Netlify，那邊會正常運行
git push origin main

# 或者本地安裝依賴
npm install
```

#### 問題 2：內容沒有更新

**原因：** 變更沒有推送到 GitHub

**解決方案：**
```bash
git status
git add .
git commit -m "更新內容"
git push origin main
# 等 2-3 分鐘讓 Netlify 重新部署
```

#### 問題 3：本地文件丟失

**這是可以預防的！** 請參考下一節的備份策略。

---

### 5. ⚠️ 關鍵：備份策略 {#zh-backup}

**這一節可能會為你節省數小時的挫折感。**

#### 問題所在

在開發過程中，你可能會不小心：
- 用 `git reset --hard` 覆蓋文件
- 在合併衝突中丟失內容
- 不小心刪除文件

**沒有備份，你的內容就沒了。**

#### 解決方案：多層備份

##### **第一層：本地資料夾備份** 💾

**這個很重要**❗**這個很重要**❗**這個很重要**❗  

每次重要的編輯完成後，備份你的整個專案資料夾：
```bash
# 基本備份指令（推薦）
cp -r my-academic-site my-academic-site-backup-$(date +%Y%m%d-%H%M)

# 如果遇到「Permission denied」錯誤，使用 rsync：
rsync -av --exclude='.git' my-academic-site/ my-academic-site-backup-$(date +%Y%m%d-%H%M)/
```

**為什麼這很重要：**
- 最直接、最可靠的備份方法
- 完整的快照，不依賴 Git
- 只需要 10 秒，能節省數小時工作
- 容易瀏覽和還原

**建議的備份時間表：**
- ✅ 每次重大內容新增後
- ✅ 任何危險的 Git 操作前
- ✅ 每次編輯結束時
- ✅ 更新 Hugo 或branch之前

**備份儲存位置：**
```bash
# 創建專門的備份資料夾
mkdir -p ~/Desktop/website-backups

# 備份到那裡
cp -r my-academic-site ~/Desktop/website-backups/backup-$(date +%Y%m%d-%H%M)
```

---

##### **第二層：Git 提交** 📦

頻繁提交：
```bash
# 編輯 1-3 個文件後
git add .
git commit -m "更新：具體描述"
git push origin main
```

**好處：**
- 版本歷史追蹤
- 可以回滾到任何時間點
- 自動同步到 GitHub

---

##### **第三層：備份分支** 🌿

重大變更前創建定期備份分支：
```bash
# 每週備份
git branch backup-weekly-$(date +%Y%m%d)
git push origin backup-weekly-$(date +%Y%m%d)

# 重大改版前
git branch backup-before-redesign
git push origin backup-before-redesign
```

---

##### **第四層：AI 對話存檔** 🤖

**當其他方法都失效時，AI 對話可以是救命稻草。**

如果你大量使用 AI 協助：

**創建里程碑快照：**
- 完成重要階段時（例如：「初始設置完成」）
- 開啟新對話並註明：「這是 [日期] 的備份對話」
- 貼上你目前完整的工作版本
- **存放在專案資料夾外** 以避免誤刪

**為什麼有效：**
- 即使本地文件丟失，AI 聊天記錄仍然存在
- 可以從對話歷史重建專案
- 記錄你的決策過程
- 遇到類似問題時可參考

**進階技巧：** 不要保存每個小程式碼片段。相反地，在達到穩定狀態時創建完整的里程碑備份。

---

#### **備份工作流程總結**
```bash
# === 日常工作流程 ===

# 1. 開始編輯
cd ~/my-academic-site

# 2. 修改內容

# 3. 本地測試（可選）
hugo server -D

# 4. 本地備份（優先級 #1 - 千萬不要跳過！）
cp -r ~/my-academic-site ~/Desktop/website-backups/backup-$(date +%Y%m%d-%H%M)

# 5. Git 提交（優先級 #2）
git add .
git commit -m "更新：你改了什麼"
git push origin main

# 6. 在 Netlify 上驗證部署

# 7.（可選）重大變更前創建備份分支
git branch backup-before-major-change
git push origin backup-before-major-change

# 8.（里程碑）必要時在 AI 對話中存檔完整版本
```

**記住：** 備份很便宜，重建丟失的工作很昂貴。本地備份是你的第一道也是最可靠的安全網。

---

### 6. 核心經驗教訓 {#zh-lessons}

**1. 跟隨官方推薦**
- 使用 Netlify（不是 GitHub Pages）
- 使用官方模板
- 初期不要過度客製化

**2. 頻繁提交**
```bash
# 編輯 1-3 個文件後
git add . && git commit -m "描述" && git push
```

**3. AI 是你的副駕駛**
- 不要猶豫尋求幫助
- 清楚地組織你的問題
- 卡住時開啟新對話
- 保留聊天記錄作為文檔

**4. 多重備份是必須的**
- 本地資料夾副本（使用 `cp` 或 `rsync`）
- Git 提交
- 備份分支
- AI 對話歷史

**5. 內容 > 技術**
- 80% 時間：優質內容
- 20% 時間：網站樣式

**6. 小步快跑**
- 分階段進行
- 持續驗證
- 不要一次做太多

---

### 7. 成功檢查清單 {#zh-checklist}

**初始設置：**
- [ ] Hugo 和 Git 已安裝
- [ ] GitHub repository 已創建
- [ ] 模板已 clone 並配置
- [ ] 已創建第一個備份
- [ ] 已部署到 Netlify
- [ ] 已設置自訂網址

**內容開發：**
- [ ] 個人資料已更新
- [ ] 研究內容已添加
- [ ] 論文列表已完成
- [ ] CV/簡歷頁面已創建
- [ ] 所有連結已測試
- [ ] 保持定期備份

**維護：**
- [ ] 備份策略已建立
- [ ] AI 對話歷史已整理
- [ ] 手機版已測試
- [ ] 已收集同儕反饋

---

### 結語

建立學術網站是一項投資：
- 💼 展示你的研究
- 🌐 建立線上存在
- 📚 整理你的工作
- 🤝 與同行交流

**核心要點：**
1. **AI 工具讓這變得可及** - 你不需要是開發者
2. **卡住時重新開始** - 新的 AI 對話提供新視角
3. **虔誠地備份** - 每次編輯後使用 `cp -r` 或 `rsync`
4. **整理你的 AI 聊天** - 它們是文檔也是備份
5. **完成 > 完美** - 先上線，再迭代

祝建站順利！🚀

---

### 關於本指南

**作者：** 孫玉婷博士  
**協助工具：** Claude AI (Anthropic)  
**最後更新：** 2025年10月30日

**網站原始碼：** [查看本網站的 GitHub repository](https://github.com/Yu-TingSun/Yu-TingSun.github.io)

---

## 相關資源

- **Hugo 文檔：** https://gohugo.io/
- **Hugo Blox 文檔：** https://docs.hugoblox.com/
- **Netlify 文檔：** https://docs.netlify.com/