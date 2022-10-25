# NovelAI prompts

**目录：**
1. [画面质量关键词](#一些提升画面质量的片段)
2. [画面风格/色调/滤镜关键词](#画面风格色调滤镜关键词)
3. [人物表情关键词](#一些调整微表情的片段)
4. [风景/静物/非人关键词](#风景静物非人关键词)
5. 光影/打光/阴影关键词
6. 人物外貌/服装/种族/设定关键词
7. 人物背景搭配/魔法特效/背景装饰关键词
8. [人物动作/姿势/角度/画面框选关键词](#人物动作姿势角度画面框选关键词)
9. [还没整理分类或者组合很有意思的整句](#一些整句)

**关于符号对prompts的影响和调整，见[wiki](https://naidb.miraheze.org/wiki/Image_Generation)**

**为了展示效果，非整句的关键词样图如无其它备注的话，都是以且仅以{{关键词}}来生成的。**

**样图自带metadata，可以下载原图并导入novelAI使用prompts或配置**

~~恐怖向的放在非人分类了~~

## 一些提升画面质量的片段

```
# 可以再加一些强调，如{{{{{masterpiece}}}}}以显著提升

masterpiece
best quality/high quality
detailed
masterwork
```
一些细碎补充：
   关于best quality/high quality等其实还有其它quality关键词（但都偏向于降低质量，具体参照[wiki](https://naidb.miraheze.org/wiki/Image_Generation)）


## 画面风格/色调/滤镜关键词

```
# 像素风。
# 我见过有人在prompts里用pixel art生成过很好看的类似于像素风游戏那种场景，用处还是很大的，不要嫌样图丑。
pixel art
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7Bpixel%20art%7D%7D%20s-1775920509.png)
```
# 草稿风。
# 这里因为加了paper所以多少可能会产出一些“像是纸上绘图”的作品，也可能会产出人物拿着纸张之类的图，如果想要排除这种干扰可以去掉paper或者给paper降低权重（[paper]）。
Sketch, paper
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7BSketch,%20paper%7D%7D%20s-369171098.png)

```
# 黑白风/素描
# 看起来更像是加了黑白滤镜的效果
black and white pencil drawing
```
![image](../pic_stoarge/NovelAi%20pic/black%20and%20white%20pencil%20drawing%20s-2015795017.png)

```
# 概念艺术。
# 我的理解是，额，概念艺术就是概念艺术嘛，适合在想要生成更奇幻的内容时添加进去。
concept/concept art
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7Bconcept%20art%7D%7D%20s-3708819849.png)
```
# 同人封面。
# 总之就是看起来很同人封面的意思，需要的时候可加，也可以在无灵感的时候加进去试试运气。（此处总会生成一些大胸奶照就不举例了免得NSFW）
doujin cover
```
```
# 长条抱枕正反面。
# 懂得都懂，但是得把画面尺寸调整到长条，横版会变成角色抱抱枕。如果你想知道怎么稳定生成反面，试试加一个{{{NSFW}}}。
body pillow concept
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7Bbody%20pillow%20concept%7D%7D%20s-2762089941.png)
```
# 复古番风
# 总之看图
1980s style
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7B1980s%20style%7D%7D%20s-1898161084.png)
```
# 木炭素描
Charcoal sketching
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7BCharcoal%20sketching%7D%7D%20s-2734295646.png)
```
# 专辑封面
# 说到专辑封面你会想到什么样的图片？对了，就是那样。
album cover
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7Balbum%20cover%7D%7D%20s-674332815.png)

```
# 颜色渐变
# 这个的用法比较多，可以做渐变的背景/衣服/头发/光效等等
Colour gradient
```
![image](../pic_stoarge/NovelAi%20pic/Colour%20gradient%20s-1302923996.png)

## 一些调整微表情的片段

**因为涉及人物表情所以为了稳定产出，一概使用“1girl, {{关键词}}, close-up, detailed face”（close-up是拉近距离，detailed face增加脸部权重），方便观察表情**

（本来是想分个喜怒哀惧爱恶欲的,但是就个人体验来说,这样分对于AI来说太细了，不一定能稳定产出。微表情这块其实挺难精准达到想要的效果，我们就简单以表情分类，不研究人物心理，不研究假笑boy。）

### 喜/乐

```
# 普通的微笑
smile/smling
```
![image](../pic_stoarge/NovelAi%20pic/1girl,%20%7B%7Bsmile%7D%7D,%20close-up,%20detailed%20face%20s-2116702852.png)

```
# 浅笑
light smile
```
![image](../pic_stoarge/NovelAi%20pic/1girl,%20%7B%7Blight%20smile%7D%7D,%20close-up,%20detailed%20face%20s-3299643682.png)

```
# 邪恶的微笑
# 要注意这里因为有个evil的关系，很大概率会影响人物，使人物带恶魔元素或者变难看。
evil smile
```
![image](../pic_stoarge/NovelAi%20pic/1girl,%20%7B%7Bevil%20smile%7D%7D,%20close-up,%20detailed%20face%20s-4044761314.png)

![image](../pic_stoarge/NovelAi%20pic/1girl,%20a%20wizard%20with%20elf%20ears,%20%7B%7Bevil-smile%7D%7D,%20detailed%20face,%20flat%20chest,%20s-3123759469.png)这里多加了一些人物设定的关键词，减轻了evil可能会导致的恶魔元素（做成平熊是防止看起来太涩涩）

```
# 一些关于smile的看不出特点但可以用的tag，兴许就玄学呢

false smile # 假笑
smiley face # 笑脸
nervous smile # 紧张的微笑，这个通过实验来看比上面那个更像假笑
crazy smile # 疯狂的微笑，没看出很疯狂但确实很露齿
forced smile # 苦笑，没看出来
sad smile # 悲伤的微笑，有一点但不多
```
```
# 普通的露齿而笑
laugh/laughing
```
![image](../pic_stoarge/NovelAi%20pic/1girl,%20%7B%7Blaughing%7D%7D,%20close-up,%20detailed%20face%20s-75078365.png)

### 怒/恶

### 哀

```
# 沉思/哀思/忧沉
# 官方举例使用的，代替“tired”。（看起来也并不怎么tired）
pensive
```
![image](../pic_stoarge/NovelAi%20pic/1girl,%20%7B%7Bpensive%7D%7D,%20close-up,%20detailed%20face%20s-2382253054.png)

```
# 哭泣
crying
```

### 惧

### 面无表情

（为什么要单独分类呢因为我觉得应该很有需求，毕竟面无表情/板着脸的绘画作品很多。）

```
emotionless
```
![image](../pic_stoarge/NovelAi%20pic/1girl,%20%7B%7Bemotionless%7D%7D,%20close-up,%20detailed%20face%20s-558398365.png)


## 风景/静物/非人关键词

### 风景
```
# 峡谷
canyon
```
### 静物
```
# 徽章/家徽
coat of arms
## 样例
Orcish {coat of arms}, gold and red, metallic, golden engraved boar heads, silver engraved mangrove trees
兽人{徽章}，金色和红色，金属，金色雕刻的野猪头，银色雕刻的红树林
```
![image](../pic_stoarge/NovelAi%20pic/Orcish%20%7Bcoat%20of%20arms%7D,%20gold%20and%20red,%20metallic,%20golden%20engraved%20boar%20heads,%20silver%20engraved%20mangrove%20trees%20s-761753710.png)

### 非人

不知道怎么说反正就是很怪的东西，这里样图不使用”{}“加重了，以免产出怪东西。
```
# 霍华德·菲利普斯·洛夫克拉夫特，简称H·P·洛夫克拉夫特，美国恐怖、科幻与奇幻小说作家
HP lovecraft
```
![image](../pic_stoarge/NovelAi%20pic/HP%20lovecraft%20s-2216368041.png)

```
# 宇宙恐怖
# 如果使用加重符号的话会增加一些星空/月亮之类的元素（但不太好看）
cosmic horror
```
![image](../pic_stoarge/NovelAi%20pic/cosmic%20horror%20s-1450316228.png)

```
# 洛夫克拉夫特式恐怖，是恐怖小说的一个子类别，着重强调未知的宇宙恐怖，而不是血腥或其他惊吓元素
Lovecraftian horror
```
![image](../pic_stoarge/NovelAi%20pic/lovecraftian%20horror%20s-501658101.png)

```
# 古怪恐怖
eldritch horror
```
![image](../pic_stoarge/NovelAi%20pic/eldritch%20horror%20s-705923851.png)

```
# 克苏鲁
# 产出大概会围绕着章鱼/软体动物生成，单看并不恐怖，只是有点掉san
cthulu
```
![image](../pic_stoarge/NovelAi%20pic/cthulu%20s-4209023468.png)

## 人物动作/姿势/角度/画面框选关键词

```
# 同一张图有多个姿势的草稿。
# 使用anatomy（解剖学）会在同一张上产出多个姿势，dynamic pose会加重不同“姿势”的权重，sketch则产出草稿风。如果嫌默认配置生成的姿势不够多，可以把画面尺寸调成横版。
Dynamic pose, sketch, anatomy 
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7BDynamic%20pose,%20sketch,%20anatomy%20%7D%7D%20s-4032864350.png)
```
# 动态角度，会产出比较超出常规姿势角度的图。
# 可以在想要调整人物角度的时候跟着姿势关键词一起加进去增加姿势权重（比如一些背身回头看之类的），也可以在毫无灵感的时候加进去看看会不会有奇妙的结果产出。
Dynamic angle
```

```
# 动态躺姿。
# 适合在尝试生成躺姿的时候使用。建议使用横版（landscape）产出图片。不然容易生成多个躺姿。
dynamic lying down pose
```
![image](../pic_stoarge/NovelAi%20pic/%7B%7Bdynamic%20lying%20down%20pose%7D%7D%20s-2486858854.png)

## 一些整句

```
# 先堆在这里后续会整理的

{Colour gradient,B&W colour mesh,high contrast,brown sketch,yellow shade,reflection in ground,glitch effect,shattered screen,Cyberpunk dystopian city,dark night, light rays, glow on edge}}}},1girl:white hair,blue eyes,white jacket,bare shoulder,slender legs,tall,hair split colour,exposed stomach,medium boobs,fight stance,holding sword,purple aura around sword,electric in sky,energy balls 
{颜色渐变，黑白彩色网格，高对比度，棕色素描，黄色阴影，地面反射，故障效果，破碎屏幕，赛博朋克反乌托邦城市，黑夜，光线，边缘发光}}}}，1girl：白发，蓝眼睛,白上衣,露肩,修长双腿,高挑,发色,露肚,中胸,格斗,持剑,剑身紫气,天电,能量球

{{{vaporwave}}}, {{neon lights}}, from below, looking down, cityscape, {{neon palette}}, starry sky, night sky, galaxy, skyscraper, on roof, 1girl, red cape, {torn cape}, black gloves, ankle boots, shorts, sitting, hands on feet, small breasts, white hair, short hair, spiky hair, brown eyes, detailed background

Upper body of beautiful female and lower body as long slender tail, covered in small scales and fins, mermaid, monster girl, 1girl

Crewmate (amongus)

ultra-realistic,{{{{by Wadim Kashin}}}},doujin cover,dynamic angle,detailled hair,absurdres,cinematic lighting,intricate details,portrait of {{{{yae miko (genshin impact)}}}} looking at viewer with a sly smile,sakura garden,pink hair,purple eyes,danbooru

Curated model

50 steps, 8 scale

Suzie, (唯@W: 1.1), {{{{{masterpiece}}}}}, {{{{best quality}}}}, {{arknights}}, 1girl, platinum hair, dark grey eyes, {{{smug}}}, medium bangs, {ponytail}, {{mole under eye}}, teenage, medium breasts, {glowing eyes}, hair between eyes, {{{{black hooded jacket}}}}, {{{{midriff peek}}}}, {{white shirt}}, black shorts, black pantyhose, {{{bandaged fingers}}}, {{{black fingerless gloves}}}, portrait, thigh pouch, {{{long sleeves}}}, {{black jacket partially removed}}, {{{black bulletproof vest}}}, waist pouches, {{{character sheet}}}, {{smirk}}

Masterpiece, night sky in background, {scattered glowing turquoise butterflies}, green grass field, detailed background, vast, {{galaxy}}, cinematic lighting, dynamic angle
Image

bedroom, small apartment, skyscraper, science fiction, no humans, far future, futuristic, high tech

hetero, couple, 1boy, 1girl, white boy, black girl, orange wavy hair, green curly hair, interracial, man yellow skin, girl green skin, sun spirit, dryad,

{large masterpiece, detailed anime, best quality, {cinematic light}, intricate details, dynamic angle, dynamic hair, {solo, 1girl}}, middle breasts, silver long hair, curly hair, {in aquarium : 3}, {{{{{{{bubbles}}}}}}}, sun light, darkness, white side slit dress, wet, from behind, hair focus, low angle, standing, in water, brilliant light, ruined castle, {{looking afar}}, {{{{bright white magic circle}}}}

(broken robot),illustration,1girl,expressionless,cold attitude,,red pupils,short hair, white hair,beautiful detailed eyes,jacket, cracked floor,damaged classroom, beautiful sky, Mechanical girl,

{dark-skinned female}, (sketch:1),limited palette,(watercolor:2.0),beautiful eyes, green eyes,{{hair flower ornament}},{detailed elegant white dress},white hair,elegant,hair between eyes,detailed scenery,{plant},front view,slightly realistic 0.1,medium hair,{focus character},hair bun,{{flower pattern}},smile,white flower, greenhouse garden,{flying beautiful butterflies}, french braid,{{wick on the shoulders}},focus face

{{Sketch, limited palette, watercolor, ink splatter,sci fi background}}, 1girl, 1boy, girl with long blonde hair fighting using a sword,girl with long white jacket,red shirt, knee socks, boy wearing black suit fighting with a gun, 1boy vs 1girl, epic fight,night sky,light rays,shadow,reflection on floor,glitch effect,red and white aura

glitter, Ophelia, suicide, rococco, red, orange, moths

hands-only, fingers, proper-anatomy.

girl {blue_fade_to_gold_hair} big_hoodie real_diamond_earrings medium_lenght_hair 2_rabbit_ears chockers {{neon_city_background}} neon_city gold_and_purple_eyes 2_hoodie_strings cyberpunk steampunk gotchic

1girl, hime cut, school uniform, hair over one eye, {black hair}, pale skin, breasts, long hair, multiple views, smirk, pantyhose, skirt lift, blazer
Undesired: pointed ears, psychedelic, error, jpeg artifacts, pointed ears, helmet, extra digits, missing fingers, blush, monochrome

Large cosmic mystic creature with near transparent wings floating in air, {scattered stars}, {{detailed background}}, cinematic lighting, masterpiece, intricate detail, {{{dramatic pose}}}, {{{dramatic angle}}}, galaxy cluster in background, grass field, night time

{{{{{{{by Paul Hedley}}}}}}}, {{{{solo}}}}, {{{1girl}}}, {{{masterpiece}}}, digital_art, {{{{{{{{{knit_turtleneck_sweater}}}}}}}}}, {{{mature women}}}, {{{{{indigo_sweater}}}}}, {{{{friendly_dark_brown_eyes}}}}, {{short_Waves_hair}}}, {{{black_hair}}}, {{{{{{{{orange_pleated_skirt}}}}}}}}, {freckles}, {{{{{very_tiny_light_smile}}}}},  {{{hands open}}} 

multicolored hair, 1girl, beautiful, small waist, realistic, ray tracing, red dress, tiara

{{solo}}, {{{{{1girl}}}}}, {{{{{{{best quality}}}}}}}, {{{{masterpiece}}}}, {{{{{{{DETAILED}}}}}}}, {{{{extremely detailed}}}}, {{{{8K wallpaper}}}}, {1girl}, 
brown eyes, glowing eyes, bright eyes, large eyes, short pink wavy hair, white head band, bangs, medium breasts, hair intakes, {{{{{loli}}}}},
{{{white tank top}}}, {{{{pink buruma}}}},
looking at viewer, {{{smile}}}, {{mouth open}},
{{fluttered detailed splash}}, water splash, blurred background, gym, sweat, cherry blossom, 
cinematic angle, cinematic lighting, {{{bokah}}}

manhwa, 1girl,{{{masterpiece}}},{{{detail}}},{{{high resolution}}},ancient china, black detailed hair, black eyes, asian,Chinese,ancient Chinese clothes, white qipao,beautiful,alluring , holding paper umbrella,Ancient palace background

Delicate facial features, {{blue_archive (Style)}}, best quality, detailed manga, detailed eyes, {cinematic light}, intricate details, dynamic angle, dynamic pose, dynamic hair, {solo, 1girl}}, night, milky way, window, white side slit dress, high hills, light silver hair, long curly hair, pink eyes, from above, eye focus, looking at viewer, star shaped hair cilp, crescent earring, standing, on bedroom

1gil, white hair, long curls, long hair, braids, {{{{{frilly maid clothes}}}}}, detached sleeves, white sleeves, {{{{{{thorny roses}}}}}}, vines, petals, black choker, ribbon choker, red eyes, pale skin, kneehigh boots, {{{{{{{short skirt}}}}}}}, black boots, Shale armor boots, chapel background, soft light, standing, looking to side, medium breasts, cleavage, {{{{{Akihiko Yoshida}}}}}, {{{Leonid Afremov}}}

1girl, pale skin, black hair, black eyes, neutral expression, white jacket, short hair, mature female, cyberpunk

1girl, black suit, black tie, black hair, messy hair, round shades with red lenses, short hair, sketch face, sketch, rough shadows, manga style

winter, elf, pale blue skin, pale blue eyes, pale blue curly hair, sad, full plate armor, winter engravings

{{{danganronpa}}}, {{portrait}}, looking at viewer, facing forward, [CHARACTER NAME HERE]

by_Wes_Anderson_propaganda_1girl

{{{action scene of: passionately smile at viewer}}},upper body,{white short shirt},1girl,red headphones,red eyes, red necktie,{{{{black trousers}}}},two-tone hair,{{{black hair}}},{{white hair}},red shoes,{{manga illustration, black-and-white, masterpiece}}{{solo, 1girl}},intricate details, character focus,{{chainsaw man(style)}}, manga (chainsaw man), demon background,{{detailed background}},{scattered glowing turquoise butterflies},{{universal gods awaken}}, cosmic horror, eldritch horror, alternate universe

{{{lalafell}}}, {{{too many frills}}}, layered dress, gown, strapless, {{{detached sleeves}}}, blonde hair, very long hair, {hair flower}, blue eyes, beautiful eyes, red eyeshadow, choker, {{{bell}}}, jewelry, curtains, window, {{{starry sky}}}, {{{full moon}}}

{{{Mori calliope:4}}}

2girls, outside, nature; red hair, long hair, sidelocks, blunt bangs, blue eyes, blush, pale skin, flat chest, grey hoodie, shorts, black leggings, brown footwear; black hair, black shorts, long hair, looking at viewer, shorts, tan, tank top, medium breasts, smile, ponytail, purple eyes

{Masterpiece}, 1guy, Plain white background. Dungeons and Dragons, fantasy, medieval.        hermit wizard.          young man, tall, 27 years old, very light skin, slender, gaunt face.          {semi long dark hair.}{{{ goatee}}}.         narrow tired eyes,  nose pointing downwards, thin lips.           tattered red cloak. dark burgundy scholar tunic.  simple attire.            art by takuji kawano and hiroaki hashimoto and shinkiro.          key visual. official work. 1990s' style. character art. vintage. retro.        Portrait. Close-up. Face. Long hair. Tattered red cloak. Brown robe.

{{{masterpiece}}}, {{{best quality}}}, {{ultra-detailed}}, {illustration}, {{an extremely delicate and beautiful}}, beautiful detailed eyes,{detailed light},{beautiful deatailed shadow}, 1girl,  {small_breasts}, floating_hair,   black hair,{painting},danganronpa(series), multi colored-hair, inner colored hair, blue hair, aqua hair, blue eyes, {{{mechanical joint, mechanical arm}}}, messy hair, makima(chainsaw man),fujimoto tatsuki, gold, bags under eyes, white clothes, hand, :/,{{{{{{surrounded by heavy floating  floating sharp fragments}}}}}},focus on face,{upper body},{{{{1girl}}}}, abstract background, {{yellow fragments around head}}, {{{mecha musume}}}, oversized clothes, melting background, pink and aqua sky

masterpiece, ultra detailed, best quality, best quality, amazing,1girl, pointy ears, finely detail, depth of field, extremely detailed CG unity 8k wallpaper, masterpiece, vampire girl, vampire element, teenager, age 18, adult style, flat chest, red hair, long twintails, red eyes, narrow eyes, pointed ears, pale skin, (beautiful detailed eyes),blood drop, blood fog, floating hair, light shafts, soft focus, character focus, dishevelled hair, looking at viewer, lowing hair, floating, splashing blood, (bloodstain), expressionless, pleated dress, no revealing clothing, bloody background, blood floating around, blood scenery, blood moon, blood sky,

A large mirror that opens a portal to space, {galaxies in mirror}, masterpiece, {{{{highly detailed}}}}, highres, casual living room in background, cinematic lighting

high_quality_background detailed_sky {rainforest} anime fantasy HD magical rain woods view_from_ground dirt moss masterpiece {{hyper_realistic}} night stars moon pond river small_fireflies best_quality clear_resolution

steampunk_hot_air_balloon_ornate_detailed

1girl, (ishida sui: 1.2),  (sketch:1), limited palette, red eyes, silver hair, shiny skin, hair between eyes, empty eyes, (lips:0.4), (watercolor:0.8), white background, (ink splatter: 1.1), from side, hair flower, (carne griffiths:1.1), red flower

1girl, floating hair, magic, lens flare, dynamic angle, portrait, solo, hidden hands, shattered glass, floating glass, glass fragments, ribbons, bowtie, hair ornament, buttons, cinematic lighting, shadows,

celestial sorceress, beautiful eyes, silver shiny hair, delicate gold crown, diamonds, glitter, dynamic angle, (ink splatter:2.5), (agnes cecile:5.5), star-lit, limited palette, pixiv (style), {{{pearlescent}}}

{{by Gaston Bussiere}}, Chiaroscuro, {{{realistic}}}, {{{art nouveau}}}, gorget, upper body, 1girl, monster girl, succubus, long hair, smile, evil, glowing eyes, blue skin, purple hair, green eyes, backlit, overbust corset, dragon wings, {{hellfire, fire background}}

1girl, solo, fire particles, white hair, short hair, curly hair (idea from myeong_chung), red eyes, burning, blue fire, serious, cinematic angle, lighting, mage,

1girl, {{{{{crystalline, made of glass, clear, transparent}}}}}, glass girl, braided hair, purple hair, {{{{{{mature}}}}}, glass eyes, green eyes, her looks will make you fall in love, photorealistic, high quality, limited palette UC: blush

Realistic, Female, robot, black sclera, sad smile, ceramic skin, bronze skin, four eyes, clockwork, goddess, steampunk, unnatural, curious, porcelain, cracked skin, doll, white skin, orokin

family crest, sigil, {{{{dragon}}}}, {{{{elvish}}}}, {{{{elegant}}}}, {{{{{{purple and black shield with golden detailing}}}}}}, {{{symmetrical}}}, {{{{family crest}}}}, {{{{coat of arms}}}}, {{{{{flowers}}}}}, {{{{black background}}}}, intricate details, dynamic lighting,

masterpiece, {{sci-fi}}, shattered glass, {{{{transhumanism, made of the future, clear, transparent}}}}, {science hexagon floor}, {{1girl, solo, red tech outfit}}, {white background},  full body, facing viewer, {{cross-section, diorama}},  comets, space, digital wire frame, anti gravity, floating, holographic face, projection, posthuman

colorized, high resolution, novigrad, the witcher

{{NaissancccceE}}, {yakumo yukari, 1girl, [mobcap], tabard, oversized clothes}, black gloves, {{high collar}}, covered mouth,{tabards collar}, white sleeves, red ribbon at elbows, close-up, pose,


UC: {{mouth mask,}} breast focus, huge breasts, slim, skin tight, collar, tail, tails


masterpiece, best quality, 4k, highres, from behind, futuristic, 1girl, {{{{{ultra detailed}}}}}, {{detailed background}}, {Ruby Rose(RWBY) on foreground}, look away, standing, science fiction, city in sky, spacecraft on background, dark grey eyes, bodysuit,  medium breasts, very wide shot, fisheye, {{{dynamic angle}}}

realistic, apocalypse barren world, fog, rain, {1girl}, detailed face, realistic eyes, young, small breasts, flat chest, white hair, very long hair, twintails, gold metal hair ornament, {white shawl}, white and black feathered wings, large wings, bright [[green]] eyes, long skirt,

{1girl}, {solo}, {{{dynamic angle}}}, {{{{dynamic hair}}}}, {{{masterpiece}}}, {{{beautiful detailed hands}}}, illustration, {{{{{beautiful detailed sky}}}}},  {{cinematic light}}, ultra detailed, {{{{{disheveld hair}}}}}, small breasts, on rooftop, pink_short_hair, curly hair, {{{hair flows upsides}}}, day, {{sun light}}, city, standing, {{{{{white_crop_tee}}}{{, {{{{yoga_skinny_pants}}}}, {{leaning breasts on handrail}}, {{{from above}}}, {{{{looking down to city}}}}, light smile, open mouth, {{{{glow_white_particles}}}}, {{{turn around}}}, falling feathers, [[[cloud]]], heart_shaped_hair_clip, simple_earring, {{{{{{pink_snapback}}}}}}, {{blue_short_jacket}}, {{{turn_back}}}, {{{beautiful_detailed_light}}}, {{high_buildings}}, {{face_toward_afar}}, {horizon}

red mage casting a colorful magic circles in the air casting a huge fire spell, red hair, light effects, magic, red mage, explosion, multicolored magic, meteor, night sky, starry sky, falling star, colors
Image

{pc-98},{mediumpixel}, {dithering}, abandoned blue factory, outside, dark night, sky, imposing, creepy, vibrant city in background 
=======
planet, city, starry sky, ecumenopolis city, star wars, Coruscant , weta digital, arial-view, city-world, city architecture, space elevator, in the wakanda concept art in artstation, vibrant, crowded, grim, skyscrapers, busy, crowds, 8k render, octane render, muted colors, central magic spire emenating energy

{masterpiece},illustration,beautiful detailed,colourful,finely detailed,intricate details,{{focus face}},{focus character},1 girl, {{white hair}},double bun hair,long hair,cyan eyes,red ribbon,{{{wet school uniform}}},short sleeve, dynamic angle,floating,beautiful detailed eyes,detailed light ,floating hair,looking at viewer,ribbon on uniform,smile,ocean in background,hold watergun,{{{{wet}}}},full body,detailed feets,no shoes


Pompt : {1girl}, {solo}, {{{dynamic angle}}}, {{{{dynamic hair}}}}, {{dynamic pose}}, {{{masterpiece}}}, {{{beautiful detailed hands}}}, illustration, {{{{{beautiful detailed nigth sky}}}}}, {{{{{beautiful-detailed eyes}}}}},  {{cinematic light}}, ultra detailed, {{{{{disheveld hair}}}}}, brown_long_hair, perm hair, {gradation eyes, (((black)))_eyes, gray_eyes}, {{halloween pumpkim}}, {{{halloween witch clothes}}}, {{frills}}, from below, looking viewer, eye focus, {moon light}, {{{{{big_orange_colored_magic_circle_on_back + mathematical_expression}}}}}, standing, {{{hair flows upsides}}}, {{{{clothes flows upsides}}}}, {{ruined castle background}}, {{expressionless}}, [[half closed eyes]], {{{{glow black eyes}}}}, {{glow orange body}}, {{{{{falling feathers foreground}}}}}, {{{{{{glowing white particles}}}}}}, small breasts, {{{{sky bubbles}}}}, {{{{light_from_back}}}}, [[lightning_on_back]]

Negative : owres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry, missing fingers, bad hands,missing arms, long neck, Humpbacked, spread legs, odd eyes

{{{by atey ghailan}}} ,{{{{{pixel art}}}}},,first person shooter, fps, pov, holding a gun, night ,gun, shooting, neon lights, action pose, cyberpunk, futuristic, science fiction, city, techwear, {{masterpiece, best quality}},  {{crowd}}

{extremely detailed CG unity 8k wallpaper}, {{masterpiece}}, {{{best quality}}}, {{ultra-detailed}}, {best illustration}, {surreal} architecture, staircase, beautiful details, cerulean blue, rococo, [[buckingham palace]], visual novel background, {{medieval}}, {{game cg}}, gothic, plants

Undesired: chandelier, lamps, people
Steps: 28
Scale: 12

{{{1girl, white hair,  blue eyes, long hair, white dress, golden trimmings, angelic wings, white thighhighs, halo, navel cutout}}}, small breasts, petite, {above clouds, sun rays}, cathedral

{{{{PSX GRAPHICS}}}}, {BEST QUALITY}}, {{MASTERPIECE}}, {{GOOD ANATOMY}}, {{CINEMATIC LIGHTING}}, {{DETAILED}}, {{TELEPHOTO LENS}},  {{PIXIV CONTEST WINNER}},{goddess}, {divine}, {{CARTOON}}, {REALISTIC}, dangerous look, {{{white eris black pupil with gold trim}}}, short black shiny hair, godly pose, unique pose, fractal horns with gold spinning up them, Prismatic claws, {{pale white skin}}, fullbody, in a fractal dimension, edgy regal cloak, pearlescent skin, edgy, regal, dynamic lighting, realistic shadows, perfect angle, hyper realistic, detailed face, detailed eyes, realistic face 


masterpiece, best quality, {{{{{illustration}}}}},,by Yuko Shimizu,1girl,chinese dragon,chinese girl,female focus on, {{color Ink wash painting}},{{ink splashing}},{{color splashing}}

{{{masterpiece}}}, {{{best quality}}}, elf, {long pointy ears}, {{{{{colored skin}}}}}, {{{{{{{green skin}}}}}}}, {{{{gradient hair}}}}, mixed colours, green curly hair, green eyes, light green curly hair, {{dark green wavy hair}}, {{{{{multicoloured hair}}}}}, {{hair flower}}, {dress}, {sleeves}, lips, {{pov}}, {{photorealistic}}, symmetry
Steps 28 Scale 5

(((masterpiece))),(((best quality))),((ultra-detailed)), ((illustration)),floating, ((an extremely delicate and beautiful)),(beautiful detailed eyes),((disheveled hair)), (painting),(sketch), 1girl, loli, small_breasts,((neck)),(((back))),(looking back), blush, sliver hair,backless dress,{{{garden}}}, {{{white flowers}}}, {{floral background}},

1boy, Masterpiece, best quality, hyper detailed, Cinematic light, intricate detail, highres, official art, high resolution illustration, finely detailed beautiful eyes, dark intense shadows, overexposure, depth of field, particle,  illustration, wildstyle, boy,  orange and blue hair, symmetrical hair color, orange hoodies, aquatic eyes, 

1girl, cigarette, balcony, confident, short hair, intricate leather jacket, punk, upper body, night, looking at camera, large shoulders, medium breasts, realistic, messy hair, rainbow hair, fireworks, symmetry, shirtless, choker, mature, adult

black and white, stylized, line art. monochrome, girl, stars

Cyril Rolando, Roberto Cavalli, a girl in a valley summoning armageddon, realistic, 1girl, vortex, swirling dust, blue hair, blue eyes, floating rocks, floating, shattered, upper body, corset, gorget, lace-trimmed shirt, poofy sleeves, magic circle, detached sleeves, medium breasts, dynamic angle, light particles

{Zdzisław Beksiński, Akihiko Yoshida}, {horror}, [3d], {{solo}}, "the angel of perception", floating head, many golden rings, {{giant red eye, third eye, light beam}}, holding ivory staff, beautiful face, very long hair, golden hair, angelic, {angel wings}, halo, clockwork

{{{masterpiece}}}, {{{best quality}}}, 1girl, {{{{{{colored skin (black)}}}}}}, {{{{{{{black skin}}}}}}}, {{{{dynamic hair (fire)}}}}, {{{{gradient hair (fire)}}}}, mixed colours, {{red flamming hair}},  orange flamming hair, {{blue flamming hair}}, {{{{{multicoloured hair (fire)}}}}}, {white dress}, {sleeves}, {{pov}}, {{{absurdres}}}, {{photorealistic}}, {{perfect eyes}}, {{detailed eyes}}, highres
Steps 28 Scale 6 Sampling k_lms

{{{{{{mixed colours}}}}}}, black, white, red, blue, 1girl,vertical symmetry, {ink splatters}, {{spilt paint}}, {{{full body}}}, {{industrial}}, {{inky hair}}, flowing hair, {{{{contrasting background}}}}, {dripping paint}

{{{viking tapestry}}},pale elven woman with long, pale green hair, {hime cut}, sidelocks with hairties, two long front locks of hair, wearing light green and brown medieval clothing, flat chest, lotr, fully clothed, neutral expression, {impasto impressionism}, [art nouveau], forehead, straight hair, nose, hair ties,

portrait,The World of Crystal,iridescent,1girl,loli,very young,Ice Goddess,solo,Ice magic, ice-flame magic,ice storm,shining eyes,jewely eyes,{{{{glint in eye}}}},Light of the moving line of sight,colorful,ice crystals clothes,ice crystals hair ornaments,dynamic pose,Dancing crystals, snow crystals,diffuse reflections,{{Masterpiece}}, {{stunning art}},  best quality, hyper detailed,beautiful, masterpiece,wind,{{dynamic angle}},{{lens flare}},beatiful detailed dark sky,{{beatiful aurora}},beatlful detailed frozen sea,{{Rainbow-colored particles}},reflective hair,good lighting,crystal tint,ray tracing,world masterpiece theater,depth of field,{ultra-detailed}, {illustration}, {detailed light｝ Amazing,beautiful detailed eyes,finely detail, extremely detailed CG,original, extremely detailed wallpaper, {an extremely delicate and beautiful},8k wallpaper

negative: lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry, long body,illust,big stomach,big breast, long neck

{{best quality castle}}, {extremely detailed CG unity 8k wallpaper}, {{{only background}}},  {{masterpiece}}, {{{best quality}}}, {{ultra-detailed}}, {best illustration}, {best shadow}, {{an extremely delicate and beautiful}}, {{{dynamic angle}}}, {{{{{glow white particles}}}}}, {{cinematic light}},  {{{in_forest}}}, {river}, day, {{sun light}}, reflection water, {{{beautiful detailed water}}}, {{bright background}}, [[sky bubbles]], {{floating calstle}}, {{falling blossom}}, {{{beautiful and delicate water}}}, {{{{{glow_pink_particles}}}}, {shine}, nature, spring, painting, falling feathers

Steps 50, Scales 3.5 ~ 7

A girl sitting on a pole in the middle of a sea, horns, suit, good composition, simplistic composition, silhouette, red moon, by Russ Mills


A 18th century painting, {{{cityscape}}}, {{{{town}}}}, {{street}}, structures, buildings, {{{{rich}}}}, fancy, luxurious, {{{{epic}}}}, beautiful, incredible, breathtaking, [[skyscrapers]], high detail, best quality, dynamic shadows, {{{{dramatic shadows}}}}, {{{{trending in artstation}}}}, {{{{{{photorealistic}}}}}}, lossless, backlighting, blending, {{ray tracing}}, {{render}}, {{surreal}}  | 18th century {{{landscape}}} painting, scenery, horizon, panorama, blue sky, {{1700's}}, [[mountainous horizon]], green fields, {{{{dramatic shadows}}}}, {{{{trending in artstation}}}}, {{{{{{photorealistic}}}}}},

1boy, Masterpiece, best quality, hyper detailed, Cinematic light, intricate_detail, highres, official art, high resolution illustration, 8k,Masterpiece, best quality, hyper detailed, Cinematic light, intricate_detail, highres, official art, high resolution illustration, 8k, dark intense shadows, beautiful detailed forest, {{black top hat, black suit, torn clothing, dark clothing}}, dark evil eyes, {{evil}}, {{{burning village}}}, insanity, screaming, {{burlap sack over head}}, crows around the character, turned head, looking at viewer, evil particles, {{dark forest}}, upper body, from above, night, {{anime}}, {{{{demonic}}}}

{{{{{masterpiece}}}}, {{summer uniform}}, side view, rain, {{{intricate details}}}, {{{{{beautiful detailed background}}}}, {{{detailed hair}}}, {{{sparkling eyes}}}, cloudy, {{{raindrops}}}, {{{cinematic lighting}}}, {{dynamic shot}}, {{illustration}} 

NAI Diffusion Anime (Full)

Steps 28, Scale 11
```


## reference

1. [官方discord](https://discord.gg/42VT8pw9)
2. [官方文档](https://docs.novelai.net/)
3. [非官方wiki-UNKB](https://naidb.miraheze.org/wiki/Main_Page)
4. [胧雨夜NovelAI](https://www.yuque.com/longyuye/lmgcwy/)
5. （**NSFW Warning**）[训练集来源danbooru](https://danbooru.donmai.us/)
6. [某位韩国玩家的prompt收录集](https://docs.google.com/document/d/11sb3AOCE4B5CZeMELNL8PwWoIae2jkrdcz-UEJw_Ayc/edit)