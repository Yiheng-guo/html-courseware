# HTML Courseware

将课程材料制作成可在浏览器演示的 HTML 课件。包含教学编排方法、1920×1080 等比舞台模板、目录和键盘翻页，以及媒体处理与交付验收规范。最新版按最终确认的浅色画布风格、封面动效与同案递进编排，并附完整示例课件。

## 使用

将本仓库克隆到 Codex 的技能目录：

```bash
git clone https://github.com/Yiheng-guo/html-courseware.git ~/.codex/skills/html-courseware
```

新开聊天后调用：

> 用 $html-courseware，把这份材料做成适合课堂投屏的 HTML 课件，面向企业业务人员，时长 30 分钟。

提供课程材料、受众、目标和时长；有品牌或参考风格时一并提供。

## 文件

- `SKILL.md`：技能入口和完整工作要求。
- `references/course-design.md`：课程编排与版式选择。
- `assets/zhaotian-prompt-courseware.html`：最终确认的完整示例课件（40 页），可直接打开对照风格。

默认面向电脑投屏；移动端阅读需求应采用流式布局。部署到公网需单独执行，生成本地文件不等于发布。
