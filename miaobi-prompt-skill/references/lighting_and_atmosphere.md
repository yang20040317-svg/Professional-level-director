# 光影与空气氛围心法（lighting_and_atmosphere.md）

光影是画面的“灵魂”。AI 生图最容易出现的“AI塑料感”往往是因为大平光、分光物理逻辑混乱所致。要生成极具立体感、电影级质感的画面，必须在提示词中**物理性地锚定光源、介质与色温**。

---

## 一、 戏剧性布光几何 (Lighting Geometry)

不要堆砌 `beautiful light`，请像一位在片场的灯光师（Gaffer）一样，明确指出光源的**位置、角度与软硬度**：

### 1. Rembrandt Chiaroscuro（伦勃朗三角光）
*   **布光结构**：主光源位于角色斜侧方约 45 度角，高度略高于人眼，副侧脸背光。
*   **物理效果**：在阴影侧的脸颊上，投射出一个明亮、完美的倒三角形光斑。
*   **情绪传达**：深邃、内敛、古典、极具戏剧性和雕刻感的面部张力。
*   **核心英文锚点**：`Rembrandt lighting, dramatic side light, Chiaroscuro, deep volumetric shadows, 45-degree key light`

### 2. High-Contrast Rim Light（高反差边缘轮廓光）
*   **布光结构**：主光源位于主体的正后方（逆光），将主体推入暗部或半剪影状态。
*   **物理效果**：沿着主体的发丝、肩部、轮廓勾勒出一道极其耀眼、剔透的亮线，使主体与黑暗的背景完美分离。
*   **情绪传达**：神圣、神秘、英雄降临、极具工业与科幻美感。
*   **核心英文锚点**：`intense rim lighting, glowing hair outline, backlight silhouette, crisp separation, dramatic halo`

### 3. Paramount / Butterfly Light（派拉蒙蝴蝶光）
*   **布光结构**：主光源位于角色正前方、正上方（约 45 度），正对着鼻梁。
*   **物理效果**：在鼻子下方投射出一个形似蝴蝶的对称阴影，同时强调颧骨和下巴线条。
*   **情绪传达**：经典好莱坞黄金时代美感。高贵、优雅、时尚、极佳的对称骨骼美。
*   **核心英文锚点**：`Butterfly lighting, Paramount light, symmetrical facial shadowing, classical Hollywood glamour`

---

## 二、 物理空气介质与粒子氛围 (Atmospheric Mediums)

光在现实世界中不是在真空中传播的，它需要穿过空气中的微小介质。描述这些**空气介质**能瞬间让扁平的画面产生极富纵深感的“空气感”：

```
     无介质（真空平光）                      有介质（体积光/丁达尔）
     [光源]                                  [光源]
       |                                     \  |  /  (体积光束)
       | (无形传播)                            \ | /
       v                                       v
   [扁平主体]                             .---'---`---. (空气颗粒反射)
                                         /   (体积雾)  \
                                        v               v
                                      [立体透射主体]
```

### 1. Tyndall Effect & Volumetric Rays（丁达尔效应 / 体积光）
*   当强光穿过充满雾气、尘埃或林木的潮湿空气时，光路会被尘埃反射，从而在空气中雕刻出清晰可见的光束（耶稣光）。
*   *英文锚点*：`Tyndall effect, visible light beams, volumetric crepuscular rays, dust motes dancing in light shaft`

### 2. Rayleigh Atmospheric Scattering（瑞利散射与大体积雾）
*   模拟大自然地平线上的空气透视。远处的山峦、建筑会因为空气的折射而逐渐变浅、变蓝，产生极强的空间层次。
*   *英文锚点*：`Rayleigh scattering, rich atmospheric haze, deep spatial depth, foggy horizon transition`

### 3. Soft Bounce Light & Global Illumination（软漫反射与全局光照）
*   光线照在地面或墙面上，会反弹回去照亮主体的背光部（如：木地板反射的金黄色微光映在墙角，水面反光的波纹投在屋檐上）。
*   *英文锚点*：`soft global illumination, ambient light bounce, environmental light reflection, subtle fill light`

---

## 三、 开尔文色温与情绪投射 (Color Temperature & Emotion)

光影的颜色能够直接唤起观者的生理与心理情感。在提示词中，可以通过**具体的自然时间段**或**物理色温（开尔文/Kelvin）**来锁定完美的影调：

### 1. Golden Hour (3000K - 3500K)
*   **时间**：日出后或日落前的 30 分钟。
*   **光影特质**：极长的拉伸阴影，温暖如蜂蜜般的金黄色侧逆光，漫反射强烈。
*   **情绪**：治愈、怀旧、希望、温馨、松弛。
*   **核心英文锚点**：`sunset golden hour light, long dramatic shadows, amber glow, 3200K warm tone illumination`

### 2. Blue Hour (6000K - 7500K)
*   **时间**：日落后至夜幕降临前的短暂时刻，太阳刚好沉入地平线。
*   **光影特质**：天空中泛着深邃忧郁的靛蓝和玫瑰红交界，几乎没有硬阴影，光线极其柔和均匀。
*   **情绪**：静谧、忧郁、神秘、孤独、浪漫。
*   **核心英文锚点**：`twilight blue hour, indigo and soft violet sky, borderless diffuse light, 7000K melancholic mood`

### 3. High-Contrast Cyberpunk Neon (3000K vs 9000K)
*   **光影特质**：强烈的色彩冲突，将极寒的荧光蓝（9000K）与灼热的霓虹粉/橙（2500K）进行冷暖对撞，营造赛博朋克夜市霓虹光影。
*   **情绪**：科幻、危险、繁华与腐朽并存、高能量。
*   **核心英文锚点**：`cyberpunk neon night, highly saturated cold cyan and warm magenta split-toning, rain-slicked street reflections`
