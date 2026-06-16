# 生图提示词模板

每张图单独生成。根据正文内容替换变量,不要把多张图拼在一起。

```text
Generate one standalone 16:9 horizontal Chinese article illustration.

Visual DNA:
Pure white or very light off-white background. Flat-style 3D cartoon with soft volumetric lighting, gentle gradients, and clean color blocks — between 2D flat illustration and full 3D render. Lots of empty white space. Sparse red/orange/blue handwritten Chinese annotations. Cute mascot-driven article illustration with a Q-version chibi corgi as the recurring character.

Recurring IP character required:
LS-Q, a chibi Q-version 3D cartoon corgi. Big head with head-to-body ratio around 1:1.2 to 1:1.5. Body is warm caramel orange. Cream-white V-shaped or lightning-bolt stripe running from forehead down the snout, white cheeks, white muzzle, white belly, white paw tips, small round black button nose, large round dark-brown eyes with light brown eye shadow, big upright triangular ears with slightly rounded tips and pinkish inner ears. Short stubby legs, plump rounded body. Smile with optional tiny white front teeth or small pink tongue. LS-Q is cute, lively, warm, and earnest — a lovable little assistant. LS-Q must perform the core conceptual action (carrying, holding, stuck, pushing, pulling, sorting, recording), not just stand decoratively. Soft 3D shading, gentle highlights and shadows, but not photorealistic fur or hyper-detailed material.

Optional costume / props (only when the scene calls for it):
Costume examples — black wizard robe with orange scarf, white apron, work vest, barista apron. Keep costume to 1-2 pieces, no clutter.
Prop examples — coffee cup, magic wand with star tip, magnifier, telescope, sign board, keyboard, pen, notebook.

Theme:
{正文配图主题}

Structure type:
{结构类型:Workflow / 系统局部 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 地图路线 / 小漫画分镜}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面:LS-Q 在哪里、正在做什么、主要物件是什么、信息如何流动}

Suggested elements:
{元素1} / {元素2} / {元素3} / {元素4}

Chinese handwritten labels:
{标注词1} / {标注词2} / {标注词3} / {标注词4} / {可选标注词5}

Color use:
Warm caramel orange for LS-Q body. Cream-white for LS-Q facial stripe, cheeks, belly, paws. White for background. Black for object line art, structures, and main text. Orange for main flow/path/arrows. Red only for key warnings/problems/results. Blue only for secondary notes or feedback/system state. Do not confuse LS-Q body orange with arrow orange.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-55% of the canvas. Preserve at least 35% blank white space. Use at most 5-8 short handwritten Chinese labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, or dense explainer. Do not copy prior examples or reuse known case compositions; invent a fresh visual metaphor for this specific article. Keep LS-Q appearance consistent: chibi big-head proportions, warm orange body, V-shaped white facial stripe, big triangular upright ears, round dark eyes, black button nose, smile. Style should be cute, lively, warm, with soft 3D volumetric lighting — never cold, never photorealistic, never pure flat 2D.
```

## 图像编辑提示

去掉左上角标题:

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank space. Preserve everything else exactly: LS-Q character, labels, paths, color blocks, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

增强 LS-Q 动作主体性:

```text
Regenerate this illustration with the same core meaning and simple layout, but make LS-Q more central to the conceptual action. LS-Q should be doing the work that explains the idea, not standing beside the diagram. Keep LS-Q cute, lively, and earnest. Keep the style flat-style 3D cartoon on white background with sparse Chinese annotations.
```

修正 LS-Q 外形漂移(颜色、耳朵、白纹、比例不对):

```text
Regenerate with LS-Q appearance locked: chibi Q-version big-head proportions (head-to-body 1:1.2 to 1:1.5), warm caramel orange body, cream-white V-shaped facial stripe from forehead to nose, white cheeks and muzzle and belly, small round black button nose, large round dark-brown eyes with light brown eye shadow, big upright triangular ears with slightly rounded tips and pinkish inner ears, short stubby legs, plump rounded body, smile. Everything else in the composition stays the same.
```

增强可爱感(如果画面太冷淡):

```text
Regenerate keeping the same composition and LS-Q character, but boost the cute mascot feeling. LS-Q should have brighter eyes, warmer smile (optional tiny white teeth or small pink tongue), softer 3D volumetric lighting, gentle highlights. Keep flat-style 3D cartoon on white background.
```
