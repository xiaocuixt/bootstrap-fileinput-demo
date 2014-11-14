bootstrap-fileinput-demo
bootstrap-fileinput应用到rails项目中
========================
<p>1. 在rails4项目中：
<p>application.js中添加： //= require fileinput.js</p>
<p>application.css中添加： *= require fileinput.css</p>
<p>2.view中表单（slim写法）：
<p>.form-group
    <p>= f.label :site_logo, 'LOGO：', class: 'col-sm-2 control-label'
    <p>.col-sm-4.container
    <p> = f.file_field :site_logo
<p>3.js调用（slim写法）：
<p>javascript:
  <p>$(function(){
    <p>$("#site_site_logo").fileinput();
  <p>});
<p>2.form中表单效果：
<p>![alt tag](http://ww4.sinaimg.cn/bmiddle/738e4c72gw1emanwtkos4j20jf09tgm6.jpg)

