# Friend Flow Apply

[friend-flow](https://github.com/AinzRimuru/friend-flow)（友链互助系统）的配置仓库，托管友链数据（`friends.yaml`）和图标资源（`icon/`）。

通过提交 PR 的方式申请添加友链。

## 申请要求

- **先行互挂**：只有已经在自己博客页面上添加了本站友链的申请才会被接受，请在 PR 中附上你的友链页面地址以便确认。
- **内容要求**：博客需保持正常更新，内容合法合规。
- **刷新间隔**：友链数据被接受后，拉取刷新间隔不得低于 **24 小时**。

## 申请方式

1. Fork 本仓库
2. 在 `friends.yaml` 末尾按照以下格式添加你的博客信息：

```yaml
- name: 你的博客名称
  url: https://your-blog.example.com/
  icon: icons/your_blog_example_com.png
  description: 一句话介绍你的博客。
  feedUrl: "https://your-blog.example.com/atom.xml"
```

3. 将你的博客图标放入 `icon/` 目录，命名为 `博客域名.png`（域名中的 `.` 替换为 `_`），建议使用方形图标，尺寸不小于 100x100 像素。
4. 提交 PR，并在 PR 描述中附上你已添加本站友链的页面地址。

## 字段说明

| 字段 | 必填 | 说明 |
|------|------|------|
| `name` | 是 | 博客名称 |
| `url` | 是 | 博客首页地址 |
| `icon` | 是 | 图标文件路径，放置在 `icon/` 目录下 |
| `description` | 是 | 一句话博客描述 |
| `feedUrl` | 否 | RSS 订阅地址，为空则自动拼接 `{url}/atom.xml` |

## 鸣谢

感谢 [LINUX DO](https://linux.do) 社区的支持。
