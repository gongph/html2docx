# html2docx
Very simple, easy to use, and the perfect Html code will be exported to Docx documents. Support custom style, say again, support custom style. I give the experience of the previous two development here to share this plug-in. Hurry Get bar!（很简单、易用、且完美的将 Html 代码导出成 Docx 文档。支持自定义样式，再说一遍，支持自定义样式。本人给予前人的经验进行二次开发的这里共享下这个插件。赶紧 Get 吧！）

Very cool jquery plugin - [html2dodcx.min.js](https://github.com/gongph/html2docx/tree/master/dist). No jQuery, or any 3rd party plugins required(不依赖任何第三方库).

## Usage(用法)

目前仅支持在 Browser globals 中使用。通过 `window.savaAsDocx(opts)` 方法导出文件。例如，像下面的代码：
```html
<script src="./dist/html2docx.min.js"></script>
<script type="text/javascript">
	  // Test
	  document.getElementById('example-btn-1').addEventListener('click', function(e){
		  saveAsDocx({
			  selector: '#example-1'
		  })
	  })
	</script>
```
## Options(参数)

`opts` 是一个 Object，下面是它所有的参数列表：

| Param | type | default | comment |
| :-----: | :-----: | :----- | :----- |
| `selector` | String | `''` | 需要导出的 DOM 元素标识。如果是 Id 选择器则传入 `'#id'`；如果是 Class 选择器则传入 `.class`；如果是 Tag 则传入 `'tag'`。[Demo](https://github.com/gongph/html2docx/blob/master/test/index.html) |
| `styleCss` | String | `''` | Css样式。样式必须放在 `<style>...</style>` 标签中。|
| `filename` | String | `Date.parse(new Date())` | 文件名 |
| `orientation` | String | `portrait` | 另一参数值：`landscape` 横向导出 |

## LICENSE
MIT License

Copyright (c) 2017 [gongph](https://github.com/gongph)
