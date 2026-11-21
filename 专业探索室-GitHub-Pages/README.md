# 专业探索室

供清沛同行志愿交流使用的静态专业探索页。包含95个专业、17个细分板块和17种培养路径样本，支持江苏高中选科设置、学习基础范围选择、偏好推荐、专业比较、目标校要求录入与记录导出。各专业含本科、硕士、博士职业路径及可核查的薪酬样本；没有可靠数字时明确注明。

93项专业及历史状态参照用户提供的清华2025级培养方案；另含农学、未来机器人两项补充。目录状态不是当前招生名单。学习基础标签不是官方选考要求，2028年江苏逐校计划尚未核验。

## 运行

直接用浏览器打开 `index.html`，无依赖、无构建步骤、无数据库。学生选择不上传，刷新后清空。

## GitHub Pages

### 用 GitHub 网页上传

1. 在自己的 GitHub 账号下新建一个公开仓库，例如 `major-explorer`。
2. 解压项目包，把 `index.html`、`.nojekyll`、`README.md`、`.gitignore` 上传到仓库根目录，不要连同外层文件夹一起上传。
3. 在仓库 Settings → Pages → Build and deployment 中选择 Deploy from a branch，分支选 `main`，目录选 `/ (root)`，保存。
4. 等待部署完成，使用 Pages 页面实际给出的地址。仓库地址用于查看代码，Pages 地址才是学生使用的网站。

### 用 Git 推送

项目包也可初始化成自己的 Git 仓库，再推送到一个新建的空仓库：

```bash
git init -b main
git add .
git commit -m "Publish major explorer"
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

把示例中的用户名和仓库名替换成自己的。若使用附带的 Git bundle，可以保留已经整理好的提交历史：

```bash
git clone major-explorer.bundle major-explorer
cd major-explorer
git remote remove origin
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

以上流程面向新建空仓库。已有仓库应先拉取现有历史再合入文件，不需要强制推送。

入口为 `index.html`，`.nojekyll` 关闭 Jekyll 处理。GitHub Pages 在中国大陆的可访问性需实测。

## 文件与版本

- `index.html`：完整独立网页，已嵌入样式、专业资料及交互脚本，下载后也可直接打开。
- `.nojekyll`：静态 Pages 配置。
- `README.md`：运行、上传与使用说明。
- `.gitignore`：忽略本机临时文件。

整理日期：2026-11-21。内容对应当前95个专业版本，不是最初的26个专业版本。

## 使用边界

推荐来自公开的标签规则，不是心理测评或报考资格判断。课程、任务为概览性归纳与示意，具体培养方案及招生条件以目标院校当年文件为准。页面内附资料入口与方法说明。
