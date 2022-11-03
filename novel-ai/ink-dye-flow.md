## 水墨-挑染-飘动

从元素法典学来的组合。

这是一代改良，主要适配官网NAI

prompt:

`masterpiece, {best quality}, Amazing, beautiful detailed eyes,{{{{1girl}}}}, finely detailed, Depth of field, extremely detailed CG unity 8k wallpaper,{{{{{full body}}}}},{{{cute animal face}}}, {{{a girl wears Clothes red Taoist robes}}}，{{Extremely gorgeous magic style}}，{{{{gold and silver lace}}}},{{{flowing lace}}},{{{flowing {{red}} and white background}}，{{{{{gorgeous detailed eyes}}}}},{{{{{{{gorgeous detail face}}}}}}},{{{{{{floating hair}}}},{{{Pick and dye red hair in white hair}}},{{{flowing transparent red}}},{{{flowing transparent white}}},{{{{{ink}}}}},{{{{small breast}}}},{{{extremely detailed gorgeous tiara}}},{{{red and white hair}}},{{red hair stick}},{{white hair ornament}},{{gold gorgeous necklace}},{{flowing hair}}，{{{{{{The picture fills the canvas}}}},{{The character is in the center of the frame}},{{{flowing}}},{{bright pupils}},{{{{melt}}}},{{{{{red and white melt}}}}}`

Undesired Content:

`{{{ugly}}},{{{duplicate}}},{{morbid}},{{mutilated}},{{{tranny}}},mutated hands,{{{poorly drawn hands}}},blurry,{{bad anatomy}},{{{bad proportions}}},extra limbs, cloned face,{{{disfigured}}},{{{more than 2 nipples}}},{{{{missing arms}}}},{{{extra legs}}},mutated hands,{{{{{fused fingers}}}}},{{{{{too many fingers}}}}},{{{unclear eyes}}},lowers, bad anatomy, bad hands,text,error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality,jpeg artifacts, signature, watermark, username, blurry, bad feet, text font ui,malformed hands, long neck, missing limb,{mutated hand and finger},{long body},{mutation poorly drawn}, disfigured, malformed mutated, multiple breasts, futa, yaoi`

`512x1024, steps 28, scales 4.5 k_euler`

可以很稳定的生成好看的图。

![image](../pic_stoarge/NovelAi%20pic/masterpiece_best_quality_Amazing_beautiful_detailed_eyes1girl_fin_s-3911190404.png)

对于我来说，我最喜欢的是它的飘动、水墨质感和少许渐变，然后好看与否大概在色彩搭配上。

所以我省略了部分内容，主要去掉了头饰，修改了一些装饰以观察效果：

![image](../pic_stoarge/NovelAi%20pic/masterpiece,%20%7Bbest%20quality%7D,%20Amazing,%20beautiful%20detailed%20eyes,%7B%7B%7B%7B1girl%7D%7D%7D%7D,%20fin%20s-3472302588(1).png)

猜测是因为有ink水墨所以飘动的碎屑（？）大多是阴阳的形状。

这里本来想通过改挑染来改变效果但是不太理想，挑染不是主要因素（就是说在b里挑染a不能稳定生成主体b）。

![image](../pic_stoarge/NovelAi%20pic/masterpiece,%20%7Bbest%20quality%7D,%20Amazing,%20beautiful%20detailed%20eyes,%7B%7B%7B%7B1girl%7D%7D%7D%7D,%20fin%20s-1153725938.png)

继续精简，只保留主体效果。去掉本来也没啥实际权重的东西。

`masterpiece, {best quality}, Amazing, beautiful detailed eyes,{{{{1girl}}}}, finely detailed, Depth of field, extremely detailed CG unity 8k wallpaper,{{{{{full body}}}}},{{{cute animal face}}}, {{{a girl wears black dress}}}，{{Extremely gorgeous magic style}}，{{{{gold and silver lace}}}},{{{flowing lace}}},{{{flowing {{red}} and white background}},{{{{{{floating hair}}}},{{{Pick and dye red hair in white hair}}},{{{flowing transparent red}}},{{{flowing transparent white}}},{{{{{ink}}}}},{{{{small breast}}}},{{{red and white hair}}},{{red hair stick}},{{flowing hair}}，{{{{{{The picture fills the canvas}}}},{{The character is in the center of the frame}},{{{flowing}}},{{bright pupils}},{{{{melt}}}},{{{{{red and white melt}}}}}`

![image](../pic_stoarge/NovelAi%20pic/masterpiece,%20%7Bbest%20quality%7D,%20Amazing,%20beautiful%20detailed%20eyes,%7B%7B%7B%7B1girl%7D%7D%7D%7D,%20fin%20s-4022740224.png)

头发挑染其实也可以去掉了，影响不大，该挑染还是会挑染。由于各种头发flow的原因，所以头发也只能跟着飘动的颜色ab跑。不能做出碎屑和头发不一样的产物

![image](../pic_stoarge/NovelAi%20pic/masterpiece,%20%7Bbest%20quality%7D,%20Amazing,%20beautiful%20detailed%20eyes,%7B%7B%7B%7B1girl%7D%7D%7D%7D,%20fin%20s-3677403988.png)

眼睛描述和表情也去掉，因为实际影响不大。（除非不做全身，但是那样各种头发飘动就没啥意义了）
（bright pulips是什么东西，没有它我的图反而更飘逸了）

小胸去掉稳定变大胸，所以干脆不去了。

{{Extremely gorgeous magic style}}, 去掉会让画面不能稳定生成合适的大幅的人。

最后精简如下：

`masterpiece, {best quality},{{{{1girl}}}}, finely detailed, Depth of field, extremely detailed CG unity 8k wallpaper,{{{{{full body}}}}}, {{{a girl wears black dress}}}，{{Extremely gorgeous magic style}},{{{{gold and silver lace}}}},{{{flowing lace}}},{{{flowing {{red}} and white background}},{{{{{{floating hair}}}},{{{flowing transparent red}}},{{{flowing transparent white}}},{{{{{ink}}}}},{{{{small breast}}}},{{flowing hair}}，{{{{{{The picture fills the canvas}}}},{{The character is in the center of the frame}},{{{flowing}}},{{{{melt}}}},{{{{{red and white melt}}}}}`

