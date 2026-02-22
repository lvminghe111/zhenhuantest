# 🎬 甄嬛传角色测试 - 图片替换指南

## 快速开始

目前测试中的图片使用的是占位符。请按下面步骤替换成《甄嬛传》角色的实际美图。

---

## 方法一：使用本地图片文件（推荐）

### 1️⃣ 准备图片
- 在项目文件夹 `C:\Users\lvminghe\zhenhuantest\` 中创建一个 `images` 文件夹
- 下载或准备如下4张高质量竖版美图（建议尺寸：400×500px 或更大）
  - `zhenhuang.jpg` - 甄嬛
  - `huafei.jpg` - 华妃
  - `huanghou.jpg` - 皇后
  - `shenmeizhang.jpg` - 沈眉庄

### 2️⃣ 更新代码
打开 `index.html`，找到下面的代码块（大约在第542-567行）：

```javascript
const characters = {
    zhenHuan: {
        name: "甄嬛",
        title: "聪慧优雅 · 命运掌控者",
        image: "https://via.placeholder.com/400x500?text=甄嬛",  // ← 修改这里
        description: "..."
    },
    ...
}
```

### 3️⃣ 替换图片URL

将以下几行中的 `image` 字段修改为：

**甄嬛：**
```javascript
image: "./images/zhenhuang.jpg",
```

**华妃：**
```javascript
image: "./images/huafei.jpg",
```

**皇后：**
```javascript
image: "./images/huanghou.jpg",
```

**沈眉庄：**
```javascript
image: "./images/shenmeizhang.jpg",
```

---

## 方法二：使用在线图片URL

如果你已经有4张角色美图的在线链接，直接替换为这些URL。例如：

```javascript
image: "https://example.com/zhenhuang.jpg",
```

---

## 💡 图片建议

### 尺寸要求
- 推荐尺寸：**400×500px** 或更大（保持竖版比例）
- 最小宽度：300px（移动端显示）

### 图片风格
- 清晰高质的角色剧照或海报
- 采用竖版构图（利于手机浏览）
- 避免过多文字遮挡
- 色调建议：暖色调或原剧照色调保持一致

### 推荐获取来源
- 🎬 小红书：搜索"甄嬛传 xx 美图"
- 📺 B站：番剧截图质量较高
- 🌐 豆瓣：电视剧相册页面
- 📸 微博：官方剧照账号

---

## 测试替换是否成功

1. 保存 `index.html` 文件
2. 刷新浏览器：`http://localhost:8888/`
3. 完成测验，查看结果页面
4. 确认显示的是真实角色美图而非占位符

---

## 常见问题

**Q: 图片加载不出来？**
A:
- 检查图片路径是否正确
- 如果使用本地文件，确保 `images` 文件夹与 `index.html` 在同级目录
- 检查文件名是否与代码中的拼写完全一致（包括大小写）
- 试试刷新浏览器 (Ctrl+F5 强制刷新)

**Q: 可以用多个角色吗？**
A: 可以！目前代码只支持这4个角色。如需添加更多角色，需修改问卷逻辑和计分系统。

**Q: 图片太大影响加载速度？**
A:
- 将图片压缩到 200-400KB 以内
- 推荐使用在线图片压缩工具：tinypng.com

**Q: 想用网络图片避免本地管理？**
A: 可以，直接用在线链接替换即可，例如：
```javascript
image: "https://cdn.example.com/zhenhuang.jpg",
```

---

## 📝 快速替换模板

复制下面的代码，替换图片URL后粘贴到代码中：

```javascript
const characters = {
    zhenHuan: {
        name: "甄嬛",
        title: "聪慧优雅 · 命运掌控者",
        image: "[这里放甄嬛图片URL]",
        description: "聪慧优雅的你，就像甄嬛一样。内心坚强，外表温柔，懂得隐忍与坚持。你用智慧和善良改变命运，即使经历伤害也能重生。你是众人的知心人，更是命运的掌控者。"
    },
    huaFei: {
        name: "华妃",
        title: "傲气十足 · 自我主宰者",
        image: "[这里放华妃图片URL]",
        description: "傲气十足的你，正如华妃一般。性格直率，气场强大，不屑于低眉顺眼。你爱恨分明，坚持自我，即使孤独也绝不妥协。你是自己人生的绝对主角。"
    },
    huangHou: {
        name: "皇后",
        title: "端庄睿智 · 权谋大师",
        image: "[这里放皇后图片URL]",
        description: "端庄睿智的你，尽得皇后之风范。理性克制，思想深远，总能看透人心。你游刃有余地处理复杂局面，用智谋而非蛮力赢得尊重。你是理性与权谋的完美化身。"
    },
    shenMeiZhuang: {
        name: "沈眉庄",
        title: "温暖善良 · 治愈使者",
        image: "[这里放沈眉庄图片URL]",
        description: "温暖善良的你，就像沈眉庄一般。心地纯良，充满同情，是朋友的知心人。你虽然温柔，但有坚守的底线。你用真诚和包容去感染身边的每一个人。"
    }
};
```

---

祝你测试顺利！ ✨
