# JavaScript-Study02
### JavaScript学习  
***********声明该资料来源于w3school以及网络博客整理，仅供学习交流谢谢！************  
HTML 中的脚本必须位于 `<script>` 与 `</script>` 标签之间。  
脚本可被放置在 HTML 页面的 `<body>` 和 `<head>` 部分中。  

#### jQuery 描述
主要的 jQuery 函数是 $() 函数（jQuery 函数）。如果您向该函数传递 DOM 对象，它会返回 jQuery 对象，带有向其添加的 jQuery 功能。
jQuery 允许您通过 CSS 选择器来选取元素。
在 JavaScript 中，您可以分配一个函数以处理窗口加载事件：  
JavaScript 方式：  
```
function myFunction()
{
var obj=document.getElementById("h01");
obj.innerHTML="Hello jQuery";
}
onload=myFunction;
等价的 jQuery 是不同的：
```  
jQuery 方式：  
```
function myFunction()
{
$("#h01").html("Hello jQuery");
}
$(document).ready(myFunction);  
```  
上面代码的最后一行，HTML DOM 文档对象被传递到 `jQuery ：$(document)`。
当您向 jQuery 传递 DOM 对象时，jQuery 会返回以 HTML DOM 对象包装的 jQuery 对象。
jQuery 函数会返回新的 jQuery 对象，其中的 `ready()` 是一个方法。
由于在 JavaScript 中函数就是变量，因此可以把 myFunction 作为变量传递给 jQuery 的 ready 方法。

