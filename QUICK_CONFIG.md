# 🖼️ 快速配置图片URL - 3步完成

## 你现在需要做什么

打开 `index.html`，找到第 **546, 552, 558, 564** 行，将以下4个 `image` 字段的URL替换为你的图片URL：

```javascript
// 第546行 - 甄嬛
image: "https://imgbed.com/upload/2024/zhenhuang.jpg",

// 第552行 - 华妃
image: "https://imgbed.com/upload/2024/huafei.jpg",

// 第558行 - 皇后
image: "https://imgbed.com/upload/2024/huanghou.jpg",

// 第564行 - 沈眉庄
image: "https://imgbed.com/upload/2024/shenmeizhang.jpg",
```

---

## 🚀 3种快速获取图片URL的方法

### 方法1：小红书 (推荐) ⭐
1. 小红书搜索：`"甄嬛传 甄嬛 高清美图"` 或 `"甄嬛传 角色剧照"`
2. 点击喜欢的图片
3. 右键 > 复制图片地址
4. 粘贴到代码中

### 方法2：图床上传（免费）
1. 访问 **sm.ms** 或 **imgur.com**
2. 上传你的4张美图
3. 复制生成的URL
4. 粘贴到代码中

**示例格式：**
```
https://sm.ms/image/xxxxx
```

### 方法3：本地图片 + 本地服务
1. 在 `C:\Users\lvminghe\zhenhuantest\` 中新建 `images` 文件夹
2. 放入4张竖版美图（jpg或png）
3. 改成相对路径：
```javascript
image: "./images/zhenhuang.jpg",
image: "./images/huafei.jpg",
image: "./images/huanghou.jpg",
image: "./images/shenmeizhang.jpg",
```

---

## 📝 完整替换示例

如果你找到的图片URL是：
```
https://example.com/zhenhuang.jpg
https://example.com/huafei.jpg
https://example.com/huanghou.jpg
https://example.com/shenmeizhang.jpg
```

在 `index.html` 中替换为：

```javascript
const characters = {
    zhenHuan: {
        name: "甄嬛",
        title: "聪慧优雅 · 命运掌控者",
        image: "https://example.com/zhenhuang.jpg",  // ← 替换这里
        description: "..."
    },
    huaFei: {
        name: "华妃",
        title: "傲气十足 · 自我主宰者",
        image: "https://example.com/huafei.jpg",  // ← 替换这里
        description: "..."
    },
    huangHou: {
        name: "皇后",
        title: "端庄睿智 · 权谋大师",
        image: "https://example.com/huanghou.jpg",  // ← 替换这里
        description: "..."
    },
    shenMeiZhuang: {
        name: "沈眉庄",
        title: "温暖善良 · 治愈使者",
        image: "https://example.com/shenmeizhang.jpg",  // ← 替换这里
        description: "..."
    }
};
```

---

## ✅ 替换完后测试

1. 保存 `index.html`
2. 刷新浏览器：http://localhost:8888/
3. 完整答题8道题目
4. 查看结果页面 - 确认显示的是你的美图！

---

## 💡 图片要求

| 要求 | 说明 |
|------|------|
| **尺寸** | 400×500px 或更大（竖版） |
| **格式** | jpg、png、webp 都支持 |
| **质量** | 清晰高质，建议小于 500KB |
| **内容** | 甄嬛传角色的剧照或美图 |

---

## 🆘 常见问题

**Q: 图片显示不出来？**
- 检查URL是否正确（不要有多余空格）
- 尝试 Ctrl+F5 强制刷新
- 检查浏览器控制台 (F12) 是否有错误

**Q: 图片加载很慢？**
- 图片可能太大，试试压缩：tinypng.com
- 或使用不同的图床源

**Q: 怎么知道URL是否有效？**
- 直接在浏览器地址栏粘贴URL
- 如果能看到图片就说明有效

---

## 📌 现在就开始！

**请提供给我以下4张图片的URL：**

1. 🎭 **甄嬛** 的美图URL：
2. 💎 **华妃** 的美图URL：
3. 👸 **皇后** 的美图URL：
4. 🌸 **沈眉庄** 的美图URL：

---

我会直接帮你配置到代码里，一键完成！✨
