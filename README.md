一、引入js和css文件
1、直接在head引入
<link rel="stylesheet" type="text/css" href="http://www.huangwx.cn/css/sweetalert.css">
<script type="text/javascript" src="http://www.huangwx.cn/js/sweetalert-dev.js"></script>
2、下载之后再引入，下载链接在文末。
 
二、js调用替代alert
直接使用swal()函数替代alert函数即可，同时sweetalert还提供更加多样化的弹出框。
 1、标准弹出框
swal("开始这个完美的弹出框旅程吧！")

2、带标题和文本的alert
swal("这是标题！","这是文本")

3、成功的提示，可以带动画效果的哦
swal("这还是标题！","这还是文本","success")
 

4、带函数传值的alert
    swal({ 
		title: "确定删除吗？", 
		text: "你将无法恢复该虚拟文件！", 
		type: "warning",
		showCancelButton: true, 
		confirmButtonColor: "#DD6B55",
		confirmButtonText: "确定删除！", 
		cancelButtonText: "取消删除！",
		closeOnConfirm: false, 
		closeOnCancel: false	
		},
		function(isConfirm){ 
		if (isConfirm) { 
			swal("删除！", "你的虚拟文件已经被删除。",
		"success"); 
		} else { 
			swal("取消！", "你的虚拟文件是安全的:)",
		"error"); 
		} 
    });

5、可以内嵌html代码的alert
    swal({ 
		title: "HTML <small>标题</small>!",
		text: "自定义<span style='color:#0000FF'>这是蓝色的<span>。", 
		html: true 
	});
摘与https://blog.csdn.net/windy1001/article/details/82685977