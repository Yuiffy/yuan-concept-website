# 元概念网站

元概念 AI 健康管理官网静态站点。

## 本地预览

直接打开 site/index.html，或使用任意静态文件服务器预览。

## 自动部署

推送到 main 分支后，GitHub Actions 会把 site/ 上传到华为云 OBS。

在仓库 Settings → Secrets and variables → Actions 中配置：

- HUAWEICLOUD_ACCESS_KEY
- HUAWEICLOUD_SECRET_ACCESS_KEY
- HUAWEICLOUD_REGION
- HUAWEICLOUD_OBS_BUCKET

建议为 GitHub Actions 单独创建华为云 IAM 用户，只授予目标 OBS 桶的必要权限。
