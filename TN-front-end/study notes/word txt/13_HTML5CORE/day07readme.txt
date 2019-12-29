文件上传方式一:[表单提交]

开发流程
1:创建目录 uploads      [保存上传文件]
2:创建表单 01_form.html [显示表单]
  #提交方式必须是 post
  GET  传递数据少[1K] 不安全
  POST 传递数据多     不安全
  #添加新属性 enctype="multipart/form-data"
  表单提交数据给服务器默认以文本方式
  将数据转换二进制文件传递
  #添加新元素 file  name="mypic"
  #添加元素   submit
3:创建php 02_upload.php [处理表单上传文件]

目录结构
day06
     uploads
     01_form.html
     02_upload.php


 特殊情况: 假设上传大于50MB文件如何处理
 如果你项目用 apache 服务器
 apache 配置文件  php.ini
 php.ini 专用于配置php程序

 a: copy php.ini ->  php01.php
 c:修改配置
 #是否允许上传操作 On/Off
 file_uploads = On    #Off 上传功能被禁止
 #上传文件大小
 upload_max_filesize = 128M
 #POST上传数据大小
 post_max_size = 130M
 指定执行php时间长度 30秒
 max_execution_time = 600
 #
 max_input_time = 600
 #指定单个php执行时内存使用最大值
 memory_limit = 135M
 memory_limit>post_max_size>upload_max_filesize


 修改完成保存，重新启动apache
 测试
 index.php     phpinfo();
















