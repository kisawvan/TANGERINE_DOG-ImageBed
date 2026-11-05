# TANGERINE_DOG ImageBed

这是 TANGERINE_DOG 的公开图片托管仓库。图片上传到这里后，可以取得公开直链并粘贴到任意 GitHub README 或 Markdown 文档中显示。

![ImageBed 示例](https://raw.githubusercontent.com/kisawvan/TANGERINE_DOG-ImageBed/main/examples/tangerine-dog-imagebed.svg)

## 上传位置

| 目录 | 用途 |
| --- | --- |
| `overview/` | 项目封面、整机外观、架构总览 |
| `hardware/` | PCB、CAN、电源、接线和调试照片 |
| `mechanical/` | 机械结构、装配和 CAD 截图 |
| `simulation/` | Gazebo、RViz、步态和 SLAM 截图 |
| `examples/` | 链接格式示例，不存放正式项目图片 |

## 最直接的使用方法

假设上传了：

```text
hardware/power-master-v1.png
```

在其他仓库的 README 中粘贴：

```markdown
![主电源管理板](https://raw.githubusercontent.com/kisawvan/TANGERINE_DOG-ImageBed/main/hardware/power-master-v1.png)
```

需要控制显示宽度：

```html
<p align="center">
  <img
    src="https://raw.githubusercontent.com/kisawvan/TANGERINE_DOG-ImageBed/main/hardware/power-master-v1.png"
    alt="主电源管理板"
    width="720">
</p>
```

也可以使用 jsDelivr CDN 链接：

```markdown
![主电源管理板](https://cdn.jsdelivr.net/gh/kisawvan/TANGERINE_DOG-ImageBed@main/hardware/power-master-v1.png)
```

Raw 链接更新后通常立即生效；CDN 可能存在缓存，更换图片内容时建议改用新的文件名。

## 获取图片直链

1. 将图片上传到本仓库对应目录。
2. 在 GitHub 中打开图片文件。
3. 点击 **Raw** 或 **Download raw file**。
4. 复制浏览器地址栏中以 `raw.githubusercontent.com` 开头的地址。
5. 将地址放入 `![图片说明](图片直链)`。

不要直接复制包含 `/blob/` 的 GitHub 文件页面地址，它是网页地址，不是图片原始文件直链。

## 文件规范

- 文件名使用小写英文、数字和连字符，例如 `single-leg-can-board-v1-1.webp`。
- 照片优先使用 WebP/JPEG，界面截图使用 PNG，矢量图使用 SVG。
- README 展示图建议不超过 1600 px，单张尽量控制在 1 MB 内。
- 不上传账号、密钥、设备序列号、个人隐私或无授权的第三方图片。
- 已经被 README 引用的图片不要随意删除；替换图片时优先使用新文件名。
