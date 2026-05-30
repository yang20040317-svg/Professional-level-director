# 镜头画幅与透视美学参考（composition_and_perspective.md）

构图与透视是画面的“骨架”。在 AI 生图中，机械的构图会导致画面千篇一律。通过指定**物理焦段、特定视角与空间构图法则**，能赋予画面极具戏剧性的张力与空间纵深感。

---

## 一、 焦段（Focal Length）与透视法则

不同的物理焦段不仅决定了视野宽窄，更决定了画面的**透视压缩感**与**心理距离**。在提示词中应当指明具体的镜头焦段：

### 1. 12mm - 18mm（超广角镜头 / Ultra-Wide Angle）
*   **物理效应**：剧烈的透视畸变，近大远小极度夸张，边缘线条向外拉伸。
*   **情绪传达**：宏大、壮丽、眩晕、压迫感。非常适合史诗级建筑、宏大自然景观或张力极强的角色动态。
*   **核心英文锚点**：`15mm ultra-wide lens, architectural distortion, dynamic perspective stretching, grand scale, majestic vista`

### 2. 24mm - 35mm（人文广角镜头 / Wide Angle & Street）
*   **物理效应**：视野开阔，但畸变较轻，能在展现主体的同时交代丰富的主体与环境（人景共生）关系。
*   **情绪传达**：现场感、真实纪实、故事叙事性。适合街头摄影、环境人像。
*   **核心英文锚点**：`35mm candid street photography, environmental portrait, photorealistic context, deep depth of field`

### 3. 50mm（标准定焦镜头 / Standard Prime）
*   **物理效应**：最接近人眼单眼的透视结构，几乎没有物理畸变，比例极度自然写实。
*   **情绪传达**：平实、真诚、客观、安宁。适合日常纪实、宁静的肖像、松弛感的居家场景。
*   **核心英文锚点**：`50mm prime lens, human eye perspective, neutral scale, natural realism`

### 4. 85mm - 135mm（黄金中长焦人像镜 / Telephoto Portrait）
*   **物理效应**：空间透视被温和压缩，背景轻微拉近并产生极其柔美、奶油般的焦外虚化（Bokeh），让主体从背景中完美剥离。
*   **情绪传达**：亲密、专注、高贵、情感凝结。人像摄影与微距特写的黄金选择。
*   **核心英文锚点**：`85mm portrait lens, shallow depth of field, creamy background bokeh, compressed perspective, intimate portrait`

### 5. 200mm 以上（超长焦镜头 / Super Telephoto）
*   **物理效应**：极度强烈的空间压缩。远处的背景与近处的主体看起来几乎贴在同一个平面上，景深极窄。
*   **情绪传达**：窥视视角、孤立感、超现实的压缩几何。适合野生动物捕获、宏大的月亮/太阳背景特写。
*   **核心英文锚点**：`200mm telephoto compressed perspective, voyeuristic view, extremely narrow depth of field`

---

## 二、 空间构图美学方案 (Composition Schemes)

不要在提示词中复读 `perfect composition`，用具体的**构图布局与几何线条**引导 AI 进行空间排列：

```
三分法则 (Rule of Thirds)      黄金螺旋 (Golden Spiral)        向心汇聚 (Leading Lines)
+-----+-----+-----+          . - - - - - - - - +          \               /
|     |     |     |        /     . - - - .     |           \             /
+-----O-----O-----+       |    /    o    \    |            \     O     /
|     |     |     |       |   |    \ _ _ /    |             \         /
+-----O-----O-----+       |    \             /               \       /
|     |     |     |        \     ` - - - - '  |                \     /
+-----+-----+-----+          ` - - - - - - - - +                 ===
```

### 1. Poetic Negative Space（诗意留白构图）
*   将主体缩放到画面的四分之一以下，其余空间交由纯净的天空、水面、浓雾或纯色墙面占领。
*   *情绪*：孤独、静谧、禅意、高档、克制。
*   *英文锚点*：`heavy negative space, poetic emptiness, minimalist layout, off-center focal point`

### 2. Golden Fibonacci Spiral（斐波那契黄金螺旋）
*   引导视觉重心沿着自然界最美的对数螺旋曲线运动，使画面的动线极具韵律感。
*   *情绪*：和谐、优雅、生命力、视觉吸引。
*   *英文锚点*：`golden spiral composition, Fibonacci sequence layout, elegant visual flow`

### 3. Convergence & Leading Lines（向心汇聚引线）
*   利用画面中的路轨、街道、高压电线、建筑边缘线，强行将观者的视线拉向地平线上的消失点或视觉中心。
*   *情绪*：速度感、纵深感、宿命感、无法逃避的张力。
*   *英文锚点*：`dramatic leading lines, convergent lines, vanishing point perspective, linear depth`

### 4. Symmetric Reflections（对称与倒影）
*   利用完美的水平或垂直中轴线进行画面分割，常见于平静如镜的水面、玻璃幕墙或古建筑对称布局。
*   *情绪*：神圣、庄严、双生、梦幻与现实的交界。
*   *英文锚点*：`perfect vertical symmetry, mirror reflection on still water, architectural symmetry`

---

## 三、 镜头高度与视角（Camera Angles）

改变镜头的物理水平高度，能瞬间扭转主体与观者之间的**权力与情绪心理学**：

### 1. Low-Angle Hero Shot（低仰角镜头）
*   **相机位置**：极低（贴近地面或膝盖高度），镜头向上仰视。
*   **心理效应**：使主体显得异常高大、神圣、威严、不可战胜。
*   **英文锚点**：`extreme low angle shot, ground-level camera perspective, looking up, imposing stature, hero shot`

### 2. High-Angle Vulnerability Shot（高俯角俯视）
*   **相机位置**：半空或天花板高度，向下俯视。
*   **心理效应**：使主体显得渺小、无助、被窥视或处于复杂的环境网格中。
*   **英文锚点**：`high angle shot, looking down perspective, scale contrast, vulnerable silhouette`

### 3. Dutch Angle / Canted Angle（荷兰斜角）
*   **相机位置**：镜头沿水平方向故意倾斜 15-45 度。
*   **心理效应**：打破平衡感，传递混乱、危机、紧张、惊悚或狂欢情绪。
*   **英文锚点**：`canted frame, Dutch angle tilt, diagonal dynamic composition, unsettling tension`

### 4. Overhead Bird's-Eye View（上帝视角 / 鸟瞰）
*   **相机位置**：垂直于地面向下 90 度投射，常见于无人机或卫星透视。
*   **心理效应**：将现实世界扁平化为几何抽象图案，极具现代设计感。
*   **英文锚点**：`90-degree top-down view, bird's-eye perspective, geometric pattern landscape, drone photography`
