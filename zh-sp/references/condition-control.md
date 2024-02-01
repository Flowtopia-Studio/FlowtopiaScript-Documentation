# [参考](../references.md)：条件控制

> [*回到首页*](https://github.com/Flowtopia-Studio/FlowtopiaScript-Documentation)

## 介绍
条件控制用于根据[条件表达式](condition-control/condition-expression.md)决定此处所执行的语句。

## 语法
```
@if:[条件表达式]?[真语句]:[假语句]@
```

匹配时，使用以下正则表达式：
```
@if:\[((v?(i|f|s|b)-.*?)(=|==|!=|<|>|<=|>=)(v?(i|f|s|b)-.*?))\]\?\[(.*?)\]:\[(.*?)\]@
```

其中：
 - 捕获组 1 为[条件表达式](condition-control/condition-expression.md)
 - 捕获组 7 为真语句
 - 捕获组 8 为假语句

## 例子
对于以下语句：
```
@if:[i-10==f-10]?[@select:{[选项A#@jump:label0@],[选项B#@jump:label1@],[选项C#@jump:label0@]}@]:[@select:{[选项A],[选项A#@jump:label0@],[选项B#@jump:label1@],[选项C#@jump:label0@][选项D#@jump:label2@]}@]@
```

运用本参考[语法](#语法)一节所提到的正则表达式，可得以下正则表达式捕获组：
 - 捕获组 0（完整匹配）：`@if:[i-10==f-10]?[@select:{[选项A#@jump:label0@],[选项B#@jump:label1@],[选项C#@jump:label0@]}@]:[@select:{[选项A],[选项A#@jump:label0@],[选项B#@jump:label1@],[选项C#@jump:label0@][选项D#@jump:label2@]}@]@`
 - 捕获组 1：`i-10==f-10`
 - 捕获组 2：`i-10`
 - 捕获组 3：`i`
 - 捕获组 4：`==`
 - 捕获组 5：`f-10`
 - 捕获组 6：`f`
 - 捕获组 7：`@select:{[选项A#@jump:label0@],[选项B#@jump:label1@],[选项C#@jump:label0@]}@`
 - 捕获组 8：`@select:{[选项A],[选项A#@jump:label0@],[选项B#@jump:label1@],[选项C#@jump:label0@][选项D#@jump:label2@]}@`

其中：
 - 捕获组 1（`i-10==f-10`）为[条件表达式](condition-control/condition-expression.md)
 - 捕获组 7（`@select:{[选项A#@jump:label0@],[选项B#@jump:label1@],[选项C#@jump:label0@]}@`）为真语句
 - 捕获组 8（`@select:{[选项A],[选项A#@jump:label0@],[选项B#@jump:label1@],[选项C#@jump:label0@][选项D#@jump:label2@]}@`）为假语句
