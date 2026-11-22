# 敬我们最亲爱的张老师

一页献给张老师的单文件网页。封面是长标题与拱形肖像，点击「点击进入」后揭开介绍页。

在线地址：<https://2012hyl.github.io/teacher-zhang/>

## 打开方式

- 直接双击 `index.html` 即可（图片走 jsDelivr CDN，离线时会自动回退到 `assets/zhang-teacher.jpg`）。
- 或在项目目录运行 `python -m http.server 8932`，访问 <http://127.0.0.1:8932/>。

## 页面内容

- 封面：敬我们 + 四行形容词 + 「张老师」+ 朱砂印章 + 「点击进入」。
- 介绍页：拱形肖像、初中历史教师、上海师范大学中国近现代史硕士；
  求学 / 实习 / 研究 / 历练 / 荣誉五段时间线；
  教学理念大引言；「世界上最好的班主任」印章与页脚。
- 学生私藏：宽容大方、温柔善良、奶茶零食三张纸条；第四张「内部资料」点开后是「直接选取正确答案法」（不告诉一般人）。点「私藏」印章还有一张头像彩蛋。
- 交互：点击进入、返回封面、Esc 返回、`#intro` 深链、滚动进度、进入时的揭页动画；「内部资料」用原生 `<details>` 展开；头像彩蛋支持 Esc / 点背景关闭。
- 适配：1440 桌面、1024 笔记本、768 平板、390 手机；`prefers-reduced-motion` 下关闭视差。

## 结构

```
index.html                 页面全部内容（HTML/CSS/JS）
assets/zhang-teacher.jpg   本地兜底肖像
preview/                   桌面与移动端预览截图
```

## 肖像地址

页面依次尝试：

1. `https://testingcf.jsdelivr.net/gh/2012hyl/imgbed@main/images/20261121_1330_zhang-teacher.jpg`
2. `https://2012hyl.github.io/imgbed/images/20261121_1330_zhang-teacher.jpg`
3. `assets/zhang-teacher.jpg`

换照片时替换第 1 条的上传路径即可；保留第 3 条可保证本地离线也能显示。

## 发布

本站由 GitHub Pages 从 `main` 分支根目录发布，推送后自动重建。
也可以把 `index.html` 与 `assets/` 放进任意静态托管（Netlify、Vercel）。
若继续用图床仓库发布，可放在子目录（例如 `zhang/`）避免覆盖图床首页。
