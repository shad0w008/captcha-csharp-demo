# ��ʾ˵��

* �������� visual studio 2015 �����棬.Net �汾 4.5.2
* ��captcha-csharp-demo.sln
* �Ҽ������������ԭNuGet��
* ���� Views\Login\Index.cshtml �ļ�
```
initNECaptcha({
  captchaId: 'YOUR_CAPTCHA_ID', // <-- �����������׶ܹ����������֤��id
  element: '#captcha_div',
  mode: 'float',
  width: '320px',
  onVerify: function(err, ret){
    if(!err){
        // ret['validate'] ��ȡ����У������
    }
  }
}, function (instance) {
  // ��ʼ���ɹ���õ���֤ʵ��instance�����Ե���ʵ���ķ���
}, function (err) {
  // ��ʼ��ʧ�ܺ󴥷��ú�����err����������ǰ������Ϣ
})
```

* ���� Controllers\LoginController.cs �ļ���������׶ܹ������뵽��������Ϣ
```
	private static string captchaId = "YOUR_CAPTCHA_ID"; // ��֤��id
	private static string secretId = "YOUR_SECRET_ID"; // ��Կ��id
	private static string secretKey = "YOUR_SECRET_KEY"; // ��Կ��key
```

* ������ʾ����
* ��ӭfork & pull request�����Ľ�Demo