һ������js��css�ļ�
1��ֱ����head����
<link rel="stylesheet" type="text/css" href="http://www.huangwx.cn/css/sweetalert.css">
<script type="text/javascript" src="http://www.huangwx.cn/js/sweetalert-dev.js"></script>
2������֮�������룬������������ĩ��
 
����js�������alert
ֱ��ʹ��swal()�������alert�������ɣ�ͬʱsweetalert���ṩ���Ӷ������ĵ�����
 1����׼������
swal("��ʼ��������ĵ������ó̰ɣ�")

2����������ı���alert
swal("���Ǳ��⣡","�����ı�")

3���ɹ�����ʾ�����Դ�����Ч����Ŷ
swal("�⻹�Ǳ��⣡","�⻹���ı�","success")
 

4����������ֵ��alert
    swal({ 
		title: "ȷ��ɾ����", 
		text: "�㽫�޷��ָ��������ļ���", 
		type: "warning",
		showCancelButton: true, 
		confirmButtonColor: "#DD6B55",
		confirmButtonText: "ȷ��ɾ����", 
		cancelButtonText: "ȡ��ɾ����",
		closeOnConfirm: false, 
		closeOnCancel: false	
		},
		function(isConfirm){ 
		if (isConfirm) { 
			swal("ɾ����", "��������ļ��Ѿ���ɾ����",
		"success"); 
		} else { 
			swal("ȡ����", "��������ļ��ǰ�ȫ��:)",
		"error"); 
		} 
    });

5��������Ƕhtml�����alert
    swal({ 
		title: "HTML <small>����</small>!",
		text: "�Զ���<span style='color:#0000FF'>������ɫ��<span>��", 
		html: true 
	});
ժ��https://blog.csdn.net/windy1001/article/details/82685977