# [参考](../references.md)：[类](../class.md) > 路径

> [*回到首页*](https://github.com/Flowtopia-Studio/FlowtopiaScript-Documentation)

## 介绍
路径是一种特殊格式的[字符串](string.md)，用于找到对应的资源。路径不包含文件扩展名。

路径会直接用于 [Unity Resources.Load(string path)](https://docs.unity3d.com/ScriptReference/Resources.Load.html) 方法中的 `path` 参数。

## 例子
以下的内容都是一个路径。
```
BackgroundMenu
```
```
Audios/Background/BackgroundMenu
```
```
Images/Character/AmamiyaRin/Smile_StreetNight
```

## 类型转换
路径可以直接被：
 - 转换为[字符串](string.md)
 - 
当满足以下格式时，路径可以被：
 - 转换为[整数](integer.md)：`\d+`
 - 转换为[浮点数](float.md)：`\d+(\.\d+)?`
 - 转换为[布尔值](bool.md)：`false|.+`
 - 转换为[标识符](mark.md) > [段落分隔符](mark/paragrath-separator.md)：`@p@`
 - 转换为[标识符](mark.md) > [换行符](mark/newline.md)：`@n@`
 - 转换为[标识符](mark.md) > [井号符](mark/hashtag.md)：`@hashtag@`
