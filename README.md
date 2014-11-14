bootstrap-fileinput-demo
bootstrap-fileinput应用到rails项目中
========================
1. 在rails4项目中：
application.js中添加： //= require fileinput.js
application.css中添加： *= require fileinput.css
2.view中表单（slim写法）：
.form-group
    = f.label :site_logo, 'LOGO：', class: 'col-sm-2 control-label'
    .col-sm-4.container
      = f.file_field :site_logo
3.js调用（slim写法）：
javascript:
  $(function(){
    $("#site_site_logo").fileinput();
  });
2.form中表单效果：
![alt tag](http://ww4.sinaimg.cn/bmiddle/738e4c72gw1emanwtkos4j20jf09tgm6.jpg)

