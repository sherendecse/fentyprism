# 万象 FENTY PRISM — 最终版 v19

对应已发布版本：2026-10-18，包含最新四款 avatar 贴纸、轮廓部位标记、常规剧本与四季盲盒。
源码提交：44222e8616dab488b0adef9b783e3e32724b9b12

## 上传 GitHub

1. 解压 ZIP。上传解压后的全部文件及文件夹，不要直接上传 ZIP。
2. 仓库顶层应直接看到 index.html、app.js、seasons.js、style.css，以及 avatars、products、fonts、vendor 等文件夹。
3. GitHub Pages 使用 main 分支、根目录 / (root)。这是纯静态网站，无需 npm、打包命令或 API key。
4. 使用 GitHub Desktop 时，将全部解压内容复制到仓库文件夹，再 Commit 和 Push。

## 文件说明

- index.html：入口
- app.js：摄像头、轮廓评估、脸型选择、剧本与收藏
- seasons.js：四季活动、36 本剧本与随机盲盒
- style.css：全部界面样式
- avatars/：四款透明头像贴纸
- products/：产品图片
- fonts/：字体与附带说明
- vendor/：农历日期库与许可证
- sources/：产品图片来源记录
- .nojekyll：让 GitHub Pages 直接发布静态文件

## 运行说明

摄像头需在 HTTPS 网站或 localhost 下使用，不建议双击 index.html 以 file:// 运行。
本地预览可在此文件夹运行 python3 -m http.server 8000，再访问 http://localhost:8000 。
脸部关键点模型首次运行需联网加载 MediaPipe 与模型资源。照片在浏览器内处理，收藏保存在当前浏览器。
四个节日目前均可预览，日期限制保持关闭。已移除所有脸型的自定义剧本入口，每种脸型保留三个正式剧本。
轮廓分析是二维照片辅助估计 Demo，结果可手动修改，并非医学或精密骨骼测量。
产品图片与品牌信息仅用于独立概念 Demo；相关商标、图片及字体遵循各自权利与许可。

## 版本完整性

网站 JS、CSS、图片、字体和农历库均与上述最终发布版本保持一致。仅将 dist 内容放到 ZIP 根目录，并加入本说明、.nojekyll 与图片来源记录，方便部署到 GitHub Pages。
