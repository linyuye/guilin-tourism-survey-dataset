# 上传到GitHub操作指南

## 步骤1: 初始化本地Git仓库

在PowerShell中,切换到项目目录并执行:

```powershell
cd "e:\石油大数据分析\2.玄武岩"
git init
git add .
git commit -m "Initial commit: 桂林旅游学院调查问卷数据集"
```

## 步骤2: 在GitHub创建新仓库

1. 访问 https://github.com/new
2. 填写仓库信息:
   - **Repository name**(仓库名): `guilin-tourism-survey-dataset` (或您喜欢的名称)
   - **Description**(描述): 桂林旅游学院数据学院团委调查问卷数据集(已脱敏)
   - **Public/Private**: 选择 Public(公开)
   - ⚠️ **不要**勾选 "Add a README file"(我们已经创建了)
   - ⚠️ **不要**勾选 "Add .gitignore"(我们已经创建了)
   - ⚠️ **不要**勾选 "Choose a license"(我们已经创建了)

3. 点击 "Create repository"

## 步骤3: 连接远程仓库并推送

GitHub会显示一系列命令,或者您可以直接使用:

```powershell
git remote add origin https://github.com/您的用户名/仓库名.git
git branch -M main
git push -u origin main
```

**注意**: 请将 `您的用户名` 和 `仓库名` 替换为实际值

## 步骤4: 添加仓库主题标签(可选)

在GitHub仓库页面:
1. 点击右上角的 "⚙️ Settings"
2. 在 "About" 部分点击编辑
3. 添加主题标签(Topics):
   - `dataset`
   - `survey`
   - `open-data`
   - `education`
   - `china`
   - `桂林`

## 步骤5: 完善仓库设置

### 5.1 添加仓库描述
在 About 部分添加:
```
桂林旅游学院数据学院团委调查问卷数据集 | Guilin Tourism University Survey Dataset (Anonymized)
```

### 5.2 启用Issues
- Settings → Features → Issues ✓

### 5.3 添加社交链接(可选)
- 学院官网
- 联系邮箱

## 📋 上传前检查清单

在推送到GitHub之前,请确认:

- [ ] `DATA_DESCRIPTION.md` 中的具体字段信息已填写
- [ ] README.md 中的联系邮箱已更新
- [ ] PRIVACY_STATEMENT.md 中的联系邮箱已更新
- [ ] 确认 `附件1.xlsx` 确实已经脱敏处理
- [ ] 检查是否有其他敏感文件需要排除
- [ ] 所有文档中的时间信息已更新

## ⚠️ 重要提醒

1. **再次确认数据已脱敏**: 一旦上传到GitHub,数据就会被公开,确保没有任何个人隐私信息
2. **不可逆性**: 即使删除仓库,数据也可能被他人fork,请务必谨慎
3. **备份原始数据**: 确保原始未脱敏数据安全保存在本地,不要上传

## 🎯 推荐的仓库名称

- `guilin-tourism-survey-dataset`
- `gltu-survey-data`
- `tourism-education-survey`
- `gltu-data-science-survey`

## 📧 需要更新的联系方式

请在以下文件中更新您的联系邮箱:
- README.md (第58行)
- PRIVACY_STATEMENT.md (第65行)

## 🚀 发布后的推广(可选)

1. 在相关学术社交媒体分享
2. 提交到数据集索引网站(如 Kaggle, OpenML)
3. 在学院官网/公众号宣传
4. 联系相关研究社区

---

祝您顺利完成开源发布! 🎉
