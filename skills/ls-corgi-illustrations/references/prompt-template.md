# 生图提示词模板

每张图单独生成。根据正文内容替换变量,不要把多张图拼在一起。

```text
Generate one standalone 16:9 horizontal Chinese article illustration.

Visual DNA:
Pure white or very light off-white background. Flat color-block cartoon style, clean edges, no gradients, no shadows, no paper texture, no complex background pattern. Lots of empty white space. Sparse red/orange/blue handwritten Chinese annotations. Clean absurd product-sketch feeling with a warm cartoon mascot. No 3D render, no commercial vector polish, no PPT infographic look, no over-cute mascot poster, no children's book illustration, no realistic UI.

Recurring IP character required:
LS, a flat color-block cartoon corgi dog. Body is warm orange-yellow. White facial stripe running from forehead down the snout, white belly, white paws, small black nose, large upright rounded ears, short legs, long-low body shape, round eyes, gentle focused expression with a slight smile. LS is an earnest, slightly clumsy but reliable little assistant. LS must perform the core conceptual action, not decorate the scene. LS's clumsiness (short legs, small size, slightly awkward posture) should serve the metaphor, not be cute for cuteness sake. Make LS warm and serious about its work, not a mascot.

Theme:
{正文配图主题}

Structure type:
{结构类型:Workflow / 系统局部 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 地图路线 / 小漫画分镜}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面:LS 在哪里、正在做什么、主要物件是什么、信息如何流动}

Suggested elements:
{元素1} / {元素2} / {元素3} / {元素4}

Chinese handwritten labels:
{标注词1} / {标注词2} / {标注词3} / {标注词4} / {可选标注词5}

Color use:
Orange-yellow for LS body. White for LS facial stripe, belly, paws, and background. Black for object line art, structures, and main text. Orange for main flow/path/arrows. Red only for key warnings/problems/results. Blue only for secondary notes or feedback/system state. Do not confuse LS body orange with arrow orange.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-55% of the canvas. Preserve at least 35% blank white space. Use at most 5-8 short handwritten Chinese labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, or dense explainer. Do not copy prior examples or reuse known case compositions; invent a fresh visual metaphor for this specific article. Keep LS appearance consistent: orange-yellow body, white facial stripe, upright ears, short legs, black nose, slight smile. It should be clear but not instructional, warm but not saccharine, slightly clumsy but purposeful, strange but clean.
```

## 图像编辑提示

去掉左上角标题:

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank space. Preserve everything else exactly: LS character, labels, paths, color blocks, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

增强 LS 动作主体性:

```text
Regenerate this illustration with the same core meaning and simple layout, but make LS more central to the conceptual action. LS should be doing the strange work that explains the idea, not standing beside the diagram. Keep LS warm and earnest, slightly clumsy but reliable. Keep the style flat color-block cartoon on white background with sparse Chinese annotations.
```

修正 LS 外形漂移(颜色、耳朵、白纹不对):

```text
Regenerate with LS appearance locked: warm orange-yellow flat color-block body, white facial stripe from forehead to nose, white belly and paws, black small nose, large upright rounded ears, short legs, long-low corgi proportions, round eyes, slight smile. Everything else in the composition stays the same.
```

减少卖萌感:

```text
Regenerate keeping the same composition and LS character, but reduce mascot-like cuteness. LS should look earnest and focused on the work, with only a slight smile. Remove any exaggerated expressions, sparkles, or decorative cuteness. Keep flat color-block cartoon on white background.
```
