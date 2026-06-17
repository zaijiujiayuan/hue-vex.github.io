# HUE-VEX

HUE-VEX VEXU 机器人团队静态首页，用于在 GitHub Pages 上提供团队统一入口。

这个页面连接团队的几个核心协作系统：

- Discourse 论坛：公告、讨论、复盘、技术问答
- Cloudreve 网盘：CAD、BOM、文档、影像和赛季资料归档
- GitHub：主页源码、公开项目和工具脚本

> Formerly IgniteForce.

## 访问地址

推荐仓库名：

```text
hue-vex.github.io
```

对应 GitHub Pages 地址：

```text
https://hue-vex.github.io
```

如果这个仓库放在个人或其他组织账号下作为项目页发布，访问路径会是：

```text
https://<owner>.github.io/hue-vex/
```

## 本地预览

这个项目没有构建步骤，直接打开 `index.html` 即可预览。

也可以启动一个本地静态服务：

```bash
python3 -m http.server 8080
```

然后访问：

```text
http://localhost:8080
```

## 修改服务链接

论坛、网盘和 GitHub 链接集中配置在 `script.js` 顶部：

```js
const serviceLinks = {
    forum: "#",
    drive: "#",
    github: "https://github.com/hue-vex"
};
```

拿到校内论坛和网盘的真实地址后，替换 `forum` 和 `drive` 即可。

## 项目结构

```text
hue-vex.github.io/
├── assets/
│   └── TeamLogo/
├── index.html
├── styles.css
├── script.js
├── LICENSE
└── README.md
```

## 设计方向

新版首页定位为团队门户，而不是宣传落地页。视觉上尽量接近论坛和网盘一类协作系统：

- 中文为主，英文作为辅助标签
- 浅色背景、白色面板、细边框、低阴影
- 第一屏突出论坛、网盘和 GitHub 三个入口
- 减少装饰动画，保持稳定、简洁、易维护

## License

MIT License. See [LICENSE](LICENSE).
