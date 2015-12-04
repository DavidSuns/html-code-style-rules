# HTML代码规范

### 1.代码风格

>* 使用soft-tab（两个空格），保证代码在各种环境下显示一致。
>* 嵌套节点应该缩进。
>* 标签名，属性名全部小写。属性值使用双引号表示，而不是单引号。
>* 不能忽略闭合标签。不用在自动闭合标签末尾使用斜线。
>* 建议一行不超过120个字符。
>* id, class的命名全部小写，并使用 “-” 分隔。
>* 元素id需保证唯一性。
>* 如果情景符合，尽量使用语义化标签。
>* 波尔类型的属性，不添加属性值。
>* 自定义属性以 XXX- 为前缀，建议使用 data-。
>* 不要滥用语义化元素，例如一个页面中出现多个h1元素。
>* 标签使用尽量简洁，减少不必要标签。
>* 不在html元素上直接注册事件，而是使用js。
>* HTML属性应该按照特定的顺序出现以保证易读性。
  >>class
  >>id, name
  >>data-*
  >>src, for, type, href, value
  >>title, alt
  >>role, aria-*
>Classes 是为高可复用组件设计的，所以他们处在第一位。Ids 更加具体而且应该尽量少使用（例如, 页内书签），所以他们处在第二位。

### 2.通用

>* 每个HTML页面使用HTML5文档声明开始标准模式，DOCTYPE 大写。
>*  启用IE EDGE模式
```html
<meta http-equiv="X-UA-Compatible" content="IE=Edge">
```
>* 指定字符编码，指定字符编码的meta标签必须是head的第一个子元素
>* 页面必须包含 title 标签申明标题，title标签需作为head的直接子元素，紧随charset声明之后。
>* 引入css和javascript时不需要指定type。
>* 在head中引入css文件。
>* 在body之后引入javascript文件，或者使用异步加载。
>* 不使用iframe。
>* 适当加入注释帮助理解。
>* 在有替代方案的情况下，不使用table进行布局。

### 3.图片

>* 为重要标签添加alt属性，对图片进行描述说明。
>* 为图片添加 width 和 height 属性，避免页面重新布局。
>* 对于图标图片，使用fonticon，svg，或者sprite图。
>* 为图片选择正确的格式。动态图使用gif格式，像素多，情景复杂的图片使用jpeg格式，其余使用png格式。
