# [参考](../../references.md)：[类](../../class.md) > [标识符](../mark.md) > 段落分隔符

> [*回到首页*](https://github.com/Flowtopia-Studio/FlowtopiaScript-Documentation)

## 介绍
段落标识符用于分割一个段落。每次点击屏幕，执行的脚本都是一整个段落。

## 例子
段落标识符的格式为`@p@`。

以下的内容都使用了段落标识符。
```
是从雨宫身上发出来的，淡淡的草莓和香橙混合的奇妙气味，明明是那么淡的味道，为什么在一瞬间放大了那么多！
@p@
而且最重要的是，她看上去平平无奇的，但是想不到，她好像，好像并不是单纯的平胸，能明显感觉到，有一点柔软的感觉压压在了我的手臂上！这和甘茉那种平板的感觉有很大不同啊！
```
```
苦匂#别，别搂着我，别搂着我！大夏天的你不嫌热吗！
@p@
实际上现在因为海水涨潮导致海风很大，整个街道都充满了凉爽的海风，真正发热的，可能是我燥热的心罢了。
@p@
这种感觉以前似乎也有过，但是实在是太久远了，已经回忆不起那时的感觉了。
@p@
@sp:ChangeBackgroundEmpty:#000000@
@sp:HideBackgroundFront@
@sp:HideBackgroundBehind@
@sp:ChangeBackgroundFront:Backgrounds/Street_Night@
@sp:ShowBackgroundFront@
@sp:ChangeCharacterMiddle:Characters/AmamiyaRin/Smile_StreetNight@
@sp:ShowCharacterMiddle@
晚上的滨临区真的很美，毕竟是沿海地区，会有很多的外地人来此观光或者定居，所以当地也很重视街道的建设，每一个店铺的窗户里都透出或温暖或炫目的光，长相端正的服务员都站在门口发送传单或者迎接客人。
```
```
穿着女仆装的开朗女生#嗯哼~
@p@
@sp:HideCharacterMiddle@
@sp:ChangeCharacterLeft:Characters/AmamiyaRin/SlightlySurprised_Blush@
@sp:ChangeCharacterRight:Characters/HaruameYuumu/Smile_OpenMouth_OpenEyes_StreetNight_Maid@
@sp:ShowCharacterLeft@
@sp:ShowCharacterRight@
突然一个穿着女仆装。满面笑容的黑头发女生站在我的面前鞠了个躬，把传单发给了我。
@p@
@sp:ChangeCharacterRight:Characters/HaruameYuumu/Smile_OpenMouth_Wink_StreetNight_Maid@
穿着女仆装的开朗女生#这位先生，有兴趣来我们餐厅里吃点东西吗？我看您家这位已经饿得不行了呢——
@p@
苦匂#什，什么？‘您家这位’是，是什么意思？！
@p@
@sp:ChangeCharacterRight:Characters/HaruameYuumu/Smile_CloseMouth_CloseEyes_StreetNight_Maid@
穿着女仆装的开朗女生#嗯？这位先生您好奇怪啊，不管怎么看她也是您的女朋友吧？贴的这么紧，真是令人羡慕啊~
@p@
果，果然被外人误会了啊啊啊啊啊啊啊！！！
@p@
@sp:ChangeCharacterRight:Characters/HaruameYuumu/Surprised_Normal_StreetNight_Maid@
苦匂#哪，哪里是！不是！她可不是啊！
@p@
@sp:HideCharacterLeft@
@sp:HideCharacterRight@
@sp:ShowCharacterMiddle@
我赶紧迈过那个女生，拖着雨宫跑走了，只留下那个女生一脸惊讶和疑惑地留在了原地。
@p@
```

## 类型转换
段落分隔符可以直接被：
 - 转换为[字符串](string.md)
 - 转换为[布尔值](bool.md)
 - 转换为[路径](path.md)
