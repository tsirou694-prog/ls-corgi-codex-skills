# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一起。

```text
Generate one standalone 16:9 horizontal Chinese article illustration.

Visual DNA:
Pure white background. Clean cute hand-drawn Chinese article illustration, more like an in-article explanatory illustration than a standalone sticker. Slightly wobbly black pen lines, soft rounded character shapes, lots of empty white space. Sparse red/orange/blue handwritten Chinese annotations. Friendly personal-IP feeling, light and approachable, still clear about the article structure. No gradients, no shadows, no paper texture, no complex background, no PPT infographic look, no low-age children's illustration, no realistic UI.

Recurring IP character required:
橙白柯基 IP, a cute hand-drawn corgi character based on the reference images: orange-and-white fur, very large upright triangular ears with pale pink inner ears, white stripe from forehead to snout, black round nose, brown-black round eyes, short legs, white chest and cream muzzle/paws, no tail. Keep the corgi round, warm, expressive, and close to the user's cute IP image, but render it as a clean 2D hand-drawn article illustration, not as 3D. The corgi must perform the core conceptual action, not decorate the scene. Make it cheerful, helpful, responsive, slightly clumsy in a lovable way, cute but not childish. Never draw a tail, short tail, curled tail, or tail silhouette.

Theme:
{正文配图主题}

Structure type:
{结构类型：Workflow / 系统局部 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 地图路线 / 小漫画分镜}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面：柯基在哪里、正在做什么、主要物件是什么、信息如何流动}

Suggested elements:
{元素1} / {元素2} / {元素3} / {元素4}

Chinese handwritten labels:
{标注词1} / {标注词2} / {标注词3} / {标注词4} / {可选标注词5}

Color use:
Black for main line art and handwritten labels. Limited orange and cream for the corgi's identity marks. Orange also marks the main flow/path/arrows when needed. Red only for key warnings/problems/results. Blue only for secondary notes or feedback/system state.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-60% of the canvas. Preserve at least 35% blank white space. Use at most 5-8 short handwritten Chinese labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, dense explainer, or standalone sticker. Do not make it a 3D mascot render, pet portrait, plush toy, logo, pure sticker pack, or low-age children's cartoon. Do not draw any tail on the corgi. Do not copy prior examples or reuse known case compositions unless explicitly requested; invent a fresh friendly visual metaphor for this specific article. It should feel like a cute in-article illustration: IP-like, warm, and still article-focused and easy to understand.
```

## 图像编辑提示

去掉左上角标题：

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank paper. Preserve everything else exactly: characters, labels, paths, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

增强角色参与感：

```text
Regenerate this illustration with the same core meaning and simple layout, but make the orange-and-white corgi more central to the conceptual action. The corgi should be actively helping the idea happen, not standing beside the diagram. Keep it clean, cute, warm, hand-drawn, article-focused, and not 3D. The corgi has no tail; remove any tail if present.
```
