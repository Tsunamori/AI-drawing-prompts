## 蝴蝶特效研究

先上初始prompts，是之前在discord收录的。

Masterpiece, night sky in background, {scattered glowing turquoise butterflies}, green grass field, detailed background, vast, {{galaxy}}, cinematic lighting, dynamic angle

512x768 steps 28 scales 7 k_euler

![啊这个已经很好看了啊](../pic_stoarge/NovelAi%20pic/Masterpiece,%20night%20sky%20in%20background,%20%7Bscattered%20glowing%20turquoise%20butterflies%7D,%20s-2930474732.png)

Masterpiece, night sky in background, {small scattered glowing butterflies}, green grass field, detailed background, vast, {{galaxy}}, cinematic lighting, dynamic angle

![横版的要把蝴蝶缩小](../pic_stoarge/NovelAi%20pic/Masterpiece,%20night%20sky%20in%20background,%20%7Bsmall%20scattered%20glowing%20butterflies%7D,%20gre%20s-1712961139.png)

但是galaxy太亮了，改一下

`Masterpiece, night sky in background, {small scattered glowing butterflies}, green grass field, detailed background, vast, [[galaxy]], cinematic lighting, dynamic angle`

![image](../pic_stoarge/NovelAi%20pic/Masterpiece,%20night%20sky%20in%20background,%20%7Bsmall%20scattered%20glowing%20butterflies%7D,%20gre%20s-2615267825.png)

既然没啥好优化的，那就把内容改一改做点别的。

去掉vast可以防止背景比重太大，同样，vast可以作出大背景小人物的效果

`Masterpiece, {{1girl}}, {{1girl wearing azure dress}}, Amazing, beautiful detailed face, floating, sleeping, flowing hair, {full body}, night sky in background, {small scattered glowing butterflies}, [[galaxy]], cinematic lighting, dynamic angle`

实践下来，closed eyes不如sleeping效果好，closed eyes很生硬，确实做不出睡着的效果

![image](../pic_stoarge/NovelAi%20pic/Masterpiece,%20%7B%7B1girl%7D%7D,%20%7B%7B1girl%20wearing%20azure%20dress%7D%7D,%20Amazing,%20beautiful%20detail%20s-444257513.png)

不知道为啥背景还是太大，要再加词。

`Masterpiece, {{1girl}}, {{1girl wearing azure dress}}, {beautiful detailed face}, {{floating}}, closed eyes, emotionless, flowing pink hair, {{full body}}, small scattered glowing butterflies, night, {{The character is in the center of the frame}}`

`Undesired Content(with default): ugly`

`768x512 steps 29 scale 10 k_euler`

差不多了，现在是稳定的状态了。
本来想做个梦中芭蕾舞的形态，但是太容易出诡异肢体了，尤其是芭蕾的脚。

![image](../pic_stoarge/NovelAi%20pic/Masterpiece,%20%7B%7B1girl%7D%7D,%20%7B%7B1girl%20wearing%20azure%20dress%7D%7D,%20%7Bbeautiful%20detailed%20face%7D%20s-1094797944.png)

![image](../pic_stoarge/NovelAi%20pic/Masterpiece,%20%7B%7B1girl%7D%7D,%20%7B%7B1girl%20wearing%20azure%20dress%7D%7D,%20%7Bcute%20anime%20face%7D,%20%7B%7Bfloa%20s-352773738.png)