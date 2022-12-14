## 神话效果研究

称之为神话的原因是原词条带有`Mythological`。

原词条（有修改）：
`1girl, solo, Mythological, deep sea, full body, fantasy, high quality, high res, intricate details, {{{intricate hair details}}}}, {{{{{beautiful detailed eyes}}}}}, {{{{{beautiful detailed background}}}}}, depth of field, detailed eyes, fine detailed hair, fine clothes, fine skin details, textile shading,`
![image](../pic_stoarge/NovelAi%20pic/1girl,%20solo,%20Mythological,%20deep%20sea,%20full%20body,%20fantasy,%20high%20quality,%20high%20res,%20s-2545919650.png)

效果比较特殊，所以单独拿出来研究一下。
如果去掉full body其实更好看一些，但这不是重点，我想知道这个复杂的线条风格是来源于什么，猜测是textile shading。

![看起来好像也不是](../pic_stoarge/NovelAi%20pic/1girl,%20solo,%20Mythological,%20deep%20sea,%20full%20body,%20fantasy,%20high%20quality,%20high%20res,%20s-3947682317.png)

保持textile shading不变，去掉Mythological看看。

![好像不能算是](../pic_stoarge/NovelAi%20pic/1girl,%20solo,%20deep%20sea,%20full%20body,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20det%20s-3356352857.png)

可能更像是几个tag的combo导致的效果。去掉不影响风格的tag看看。

`Mythological, fantasy, high quality, high res, intricate details, {{{intricate hair details}}}}, {{{{{beautiful detailed eyes}}}}}, {{{{{beautiful detailed background}}}}}, depth of field, detailed eyes, fine detailed hair, fine clothes, fine skin details, textile shading,`

![以这个为基准开始删tag](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20details,%20%7B%7B%7Bintricate%20h%20s-1150470811.png)

去掉depth of field

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20details,%20%7B%7B%7Bintricate%20h%20s-1150470811%20(copy%201).png)

去掉{{{{{beautiful detailed eyes}}}}}

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20details,%20%7B%7B%7Bintricate%20h%20s-1150470811%20(copy%202).png)

去掉{{{{{beautiful detailed background}}}}}

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20details,%20%7B%7B%7Bintricate%20h%20s-1150470811%20(copy%203).png)

去掉 {{{intricate hair details}}}}

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20details,%20detailed%20eyes,%20s-1150470811.png)

detailed eyes

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20details,%20fine%20detailed%20s-1150470811.png)

fine detailed hair

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20details,%20fine%20clothes,%20s-1150470811.png)

fine skin details, 由产出可见这个tag加重了人脸的比重。

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20intricate%20details,%20fine%20clothes,t%20s-1150470811.png)

intricate details, 

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,fine%20clothes,textile%20shading,%20s-1150470811.png)

,fine clothes，看产物，去掉了clothes会导致间接失去人的产出。

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,textile%20shading,%20s-1150470811.png)

textile shading, 失去针织品权重。

![image](../pic_stoarge/NovelAi%20pic/Mythological,%20fantasy,%20high%20quality,%20high%20res,%20s-1150470811.png)

Mythological, 

![image](../pic_stoarge/NovelAi%20pic/fantasy,%20high%20quality,%20high%20res,%20s-1150470811.png)

fantasy, 这里人的权重又回来了应该是因为原图有人。

![image](../pic_stoarge/NovelAi%20pic/high%20quality,%20high%20res,%20s-1150470811.png)

整理一下，实际上最核心的tag是fantasy，如果要画人，可以使用`Mythological, fantasy, high quality, high res, intricate details, {{{intricate hair details}}}}, {{{{{beautiful detailed eyes}}}}}, {{{{{beautiful detailed background}}}}}, depth of field, detailed eyes, fine detailed hair, fine clothes, fine skin details, textile shading,`，如果要画全身+背景，可以去掉fine skin details。如果想画非人的景物，可以用`Mythological, fantasy, high quality, high res, intricate details, {{{{{beautiful detailed background}}}}}, depth of field, textile shading,`，depth of field可以看情况去掉。

那么最后，结合以前的人鱼研究尝试搞个人鱼试试。

`masterpiece, {best quality}, finely detailed, Depth of field, extremely detailed CG unity 8k wallpaper, 1girl, Upper body of beautiful female and lower body as long {{slender}} mermaid tail, covered in small scales, floating hair, bubbles, under water, floating transparent ribbons, {{The character is in the center of the frame}}, Mythological, deep sea, fantasy, high quality, high res, intricate details, {{{intricate hair details}}}}, {{{{{beautiful detailed eyes}}}}}, {{{{{beautiful detailed background}}}}}, depth of field, detailed eyes, fine detailed hair, fine clothes, fine skin details, textile shading,`

![image](../pic_stoarge/NovelAi%20pic/masterpiece,%20%7Bbest%20quality%7D,%20finely%20detailed,%20Depth%20of%20field,%20extremely%20detailed%20s-1667880003.png)

最后做了一下调整，可以稳定得到水下的漂亮人物（除了尾巴）。

masterpiece, {best quality}, finely detailed, Depth of field, extremely detailed CG unity 8k wallpaper, 1girl, Upper body of beautiful female and lower body as long {slender} {mermaid tail}, covered in small scales, bubbles, under water, [floating transparent ribbons], {{The character is in the center of the frame}}, Mythological, deep sea, fantasy, high quality, high res, intricate details, {{{{{beautiful detailed eyes}}}}}, {{{{{beautiful detailed background}}}}}, depth of field, detailed eyes, fine detailed hair, fine clothes, fine skin details, textile shading,

step 28 scale 11 k_euler

nc: ugly, multi tails

![image](../pic_stoarge/NovelAi%20pic/masterpiece,%20%7Bbest%20quality%7D,%20finely%20detailed,%20Depth%20of%20field,%20extremely%20detailed%20s-961541842.png)

使用NAI diffusion的curated模型试了下，去掉了人鱼描述，scale 11
这个模型相对来说确实更好看一些，但人脸貌似有点单调。
![image](../pic_stoarge/NovelAi%20pic/masterpiece,%20%7Bbest%20quality%7D,%20finely%20detailed,%20Depth%20of%20field,%20extremely%20detailed%20s-3703327701.png)

scale 4.5

![image](../pic_stoarge/NovelAi%20pic/masterpiece,%20%7Bbest%20quality%7D,%20finely%20detailed,%20Depth%20of%20field,%20extremely%20detailed%20s-502007984.png)

## fantasy tag 研究

既然确定了主要效果来自fantasy，把它和一些其他风格结合一下有没有什么好看的效果。

首先做一个初始图像取seed做后续对比。

`masterpiece, 1girl, purple curly hair, white dress, `

![seed:3838361589](../pic_stoarge/NovelAi%20pic/masterpiece,%201girl,%20purple%20curly%20hair,%20white%20dress,%20s-3838361589.png)

加上fantacy。

![masterpiece, fantasy, 1girl, purple curly hair, white dress, ](../pic_stoarge/NovelAi%20pic/masterpiece,%20fantasy,%201girl,%20purple%20curly%20hair,%20white%20dress,%20s-3838361589.png)

变化不大，把scale调低到4.5，提升变化。

![scale4.5](../pic_stoarge/NovelAi%20pic/masterpiece,%20fantasy,%201girl,%20purple%20curly%20hair,%20white%20dress,%20s-3838361589%20(copy%201).png)

![fantasy, melt metal](../pic_stoarge/NovelAi%20pic/masterpiece,%20fantasy,%201girl,%20purple%20curly%20hair,%20white%20dress,%20s-3838361589%20(copy%201).png)

## 一些神话系人设尝试

从看到这个风格的时候，就想做一些类似于库洛牌的效果。

