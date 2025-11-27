# xiatianchichichi.github.io

# ✏️ 自定义指南

## 1️⃣ 修改基本信息

```html
<!-- 导航栏 -->
<span class="nav-name">Your Name</span>

<!-- 头像 -->
<div class="profile-photo">YN</div>  <!-- 字母缩写 -->
<!-- 或用真实照片 -->
<div class="profile-photo"><img src="photo.jpg" alt=""></div>

<!-- 姓名 -->
<h1>Your Name <span class="cn-name">(中文名)</span></h1>

<!-- 职位 -->
<p class="profile-position">
    博士，副教授，硕士生导师<br>
    某某大学 计算机学院
</p>
```

## 2️⃣ 新闻动态

```html
<div class="news-item">
    <span class="news-date">2025.11</span>
    <span class="news-content">
        <span class="news-tag accept">录用</span>
        论文被 <span class="news-highlight">AAAI 2026</span> 录用！
    </span>
</div>
```

**标签类型：**
| 类名 | 颜色 | 用途 |
|-----|------|-----|
| `news-tag accept` | 绿色 | 论文录用 |
| `news-tag award` | 橙色 | 获奖 |
| `news-tag talk` | 蓝色 | 报告/演讲 |

## 3️⃣ 添加论文

```html
<div class="pub-item">
    <div class="pub-title"><a href="链接">论文标题</a></div>
    <div class="pub-authors">作者1, <span class="me">你的名字*</span>, 作者3</div>
    <div class="pub-venue">期刊/会议名, 年份.</div>
    <div class="pub-tags">
        <span class="pub-tag sci-1">SCI一区</span>
        <span class="pub-tag ccf-a">CCF A</span>
    </div>
    <div class="pub-links">
        <a href="#" class="pub-link">[Paper]</a>
        <a href="#" class="pub-link">[Code]</a>
    </div>
</div>
```

**论文标签：**
| 类名 | 颜色 | 用途 |
|-----|------|-----|
| `pub-tag ccf-a` | 红色 | CCF A类 |
| `pub-tag ccf-b` | 橙色 | CCF B类 |
| `pub-tag ccf-c` | 靛蓝 | CCF C类 |
| `pub-tag sci-1` | 绿色 | SCI一区 |
| `pub-tag sci-2` | 青色 | SCI二区 |
| `pub-tag esi` | 紫色 | ESI高被引 |
| `pub-tag oral` | 蓝色 | Oral |
| `pub-tag spotlight` | 粉色 | Spotlight |

## 4️⃣ 学生培养

```html
<div class="student-year">
    <span class="student-year-badge">2024级</span>
    <div class="student-names">
        学生A、学生B <span class="student-award">国奖</span>、学生C
    </div>
</div>
```

**学生标签：**
- `<span class="student-award">国奖</span>` - 橙色标签
- `<span class="student-note">(已毕业)</span>` - 灰色备注

## 5️⃣ 修改主题颜色

```css
:root {
    --primary: #2563eb;        /* 主色调（蓝色） */
    --accent: #059669;         /* 强调色（绿色） */
    --warning: #dc2626;        /* 警告色（红色） */
}
```

# 📁 包含模块

| 模块 | 说明 |
|-----|-----|
| Profile | 简洁开头 |
| News | 带标签的新闻动态 |
| Publications | 按方向分类的论文 |
| Projects | 科研项目列表 |
| **Students** | **学生培养（已启用）** |
| Awards | 荣誉奖项 |
| Services | 学术服务 |

# 💡 提示

- 用 `<span class="me">` 高亮自己的名字
- 通讯作者在名字后加 `*`
- 本科生可标注 `(本科生)`
- 学生获奖用 `<span class="student-award">` 标签
