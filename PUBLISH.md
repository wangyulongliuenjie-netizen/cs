# 🚀 网站发布指南

## 📦 文件清单

你的网站包含以下文件：

```
index.html          → 主页（展示用）
admin.html          → 后台编辑管理页面 ✨ NEW
site-data.js        → 网站内容配置（自动生成）
thank-you.html      → 表单提交后的感谢页
css/styles.css      → 样式表
js/script.js        → 脚本
README.md           → 说明文档
```

---

## 🌐 方案对比

| 方案 | 难度 | 费用 | 自动更新 | 推荐度 |
|------|------|------|--------|--------|
| **GitHub Pages** | ⭐⭐ | 免费 | 手动 | ⭐⭐⭐⭐⭐ |
| Netlify | ⭐⭐⭐ | 免费 | 自动 | ⭐⭐⭐⭐ |
| Vercel | ⭐⭐⭐ | 免费 | 自动 | ⭐⭐⭐⭐ |
| 传统主机 | ⭐⭐⭐⭐ | 付费 | 手动 | ⭐⭐ |

---

## ✅ 推荐方案：GitHub Pages（最简单）

### 第一步：创建 GitHub 账户（5分钟）
1. 访问 https://github.com/signup
2. 填写邮箱、密码、用户名（如：`your-username`）
3. 验证邮件

### 第二步：创建仓库
1. 登录 GitHub
2. 点击 **`+`** 旁的下拉箭头 → **New repository**
3. 仓库名填写：**`your-username.github.io`**
   - 例如：如果用户名是 `alice`，就填 `alice.github.io`
4. 选择 **`Public`** 公开
5. 点击 **Create repository**

### 第三步：上传文件
有两种方式选一种：

#### 方式A：Web 上传（最简单）
1. 打开你刚创建的仓库
2. 点击 **Add file** → **Upload files**
3. 把这些文件拖到框里：
   - `index.html`
   - `admin.html`
   - `site-data.js`
   - `thank-you.html`
   - `css/` 文件夹
   - `js/` 文件夹
4. 点击 **Commit changes**

#### 方式B：用 Git 上传（稍专业）
```bash
# 1. 安装 Git（https://git-scm.com/）

# 2. 在本地建立文件夹
mkdir my-site && cd my-site

# 3. 复制所有网站文件到这个文件夹

# 4. 执行以下命令
git init
git add .
git commit -m "首次提交"
git branch -M main
git remote add origin https://github.com/your-username/your-username.github.io.git
git push -u origin main
```

### 第四步：访问你的网站
浏览器打开：`https://your-username.github.io`

> 💡 **提示**：可能需要等 1-2 分钟才能生效

---

## ✏️ 如何编辑内容

### 方法1️⃣：用后台编辑器（最方便！）
1. 打开 `https://your-username.github.io/admin.html`
2. 填写表单修改内容
3. 点击 **"💾 保存配置"** 自动下载新的 `site-data.js`
4. 刷新页面查看效果

### 方法2️⃣：直接编辑 site-data.js（需要代码知识）
1. 在 GitHub 上找到 `site-data.js` 文件
2. 点击铅笔图标编辑
3. 修改内容
4. 点击 **Commit changes**

---

## 📝 编辑内容说明

打开 `admin.html` 可以编辑：

- **👤 基本信息**
  - 姓名、职位、所在地、工作经验、专注领域、邮箱

- **🏷️ 顶部标签**
  - 显示在最上面的小标签（如：Designer, Developer）

- **🚀 英雄标题**
  - 大标题的三行（如：创造 / 有意义的 / 作品与体验）

- **🎯 卡片信息**
  - 欢迎卡片的 Emoji、标题、描述

- **📖 个人简介**
  - 三段关于你的介绍

- **📊 统计数据**
  - 显示的各类数据（如：5 年经验）

- **🔗 社交链接**
  - 你的 Twitter、LinkedIn 等

- **🤝 合作伙伴**
  - 合作过的公司、品牌

---

## 🎯 完整编辑流程

```
1. 打开 admin.html
   ↓
2. 填写表单修改内容
   ↓
3. 点击"保存配置"（自动下载 site-data.js）
   ↓
4. 上传新的 site-data.js 到 GitHub
   ↓
5. 等待 1-2 秒，刷新网站查看效果
```

---

## 🔒 隐私建议

如果不想公开源代码（出于隐私或竞争考虑）：

1. GitHub 仓库改为 **Private** 私有
2. 在仓库 Settings → Pages 中选择 **public** 发布
3. 网站可以公开访问，但代码只有你能看到

---

## 🚨 常见问题

**Q: 修改后为什么没有立即更新？**
A: 网站通常需要 1-2 秒才能更新。试试：
- 等10秒再刷新
- Ctrl+Shift+Delete 清除缓存后刷新
- 用无痕窗口测试

**Q: 能否添加数据库和动态功能？**
A: 这个版本是静态网站。如果需要数据库可以用：
- Netlify Forms（表单收集）
- Google Sheets + 脚本（内容管理）
- Firebase（超强大）

**Q: 表单能收集用户提交的信息吗？**
A: 目前表单跳转到感谢页。要真正收集需要：
- 用 Netlify 的免费表单功能
- 用 Formspree（免费表单后端）
- 用 Google Sheets 作后端

**Q: 支持自定义域名吗？**
A: 支持！在 GitHub settings → Custom domain 中配置。
需要改 DNS。详见：https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

---

## 🎓 下一步优化（可选）

如果想要更强大的功能：

1. **SEO 优化**：添加 meta 标签
2. **统计分析**：集成 Google Analytics
3. **表单收集**：用 Netlify Forms
4. **自动化部署**：GitHub Actions
5. **CDN 加速**：用 Cloudflare

---

## 📞 需要帮助？

如有问题，联系我或查看官方文档：
- GitHub Pages：https://pages.github.com/
- Git 教程：https://github.com/skills/introduction-to-github

---

**准备好了吗？现在就发布你的网站吧！🚀**
