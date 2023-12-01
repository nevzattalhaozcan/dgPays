# Görev

• Çalışmayla ilgili doküman linki: https://documenter.getpostman.com/view/24419403/2s8ZDbWgPN

• Mock url: https://787b4ca6-3ce1-4903-8150-90acc1c59914.mock.pstmn.io

• Authorization tab'ında type API Key seçildikten sonra key field'ına "x-api-key" yazılmalı. Value kısmına ise api key yazılmalıdır. Bu "API Key" mail olarak paylaşılacaktır. Add to field kısmı "Header" seçildikten sonra çalışma yapılmalıdır.c

Yeni bir collection oluşturup sadece bu collection üzerinden çalışma yapılmasını bekliyoruz. Bu collection'ında, body ve response'lar JSON formatına göre oluşturulup kontrol edilmesi, tek bir 'Post' metodu ile Post - Get - Put - Delete metotları bir request altında olacak şekilde kullanılmasını ve case yazımının test tab'ında olması beklenmektedir. Bir nesne oluşturup nesne içerisinde fonksiyonların tanımlanmasını ve bu fonksiyonların body'de kullanılmasını bekliyoruz. Request gönderilip response'da dönen key value'lara göre soruların cevapları beklenmektedir. 

• Değişkenler pre-request script tab'ında tanımlanmalıdır.

• Test tab'ında ise tek bir 'Post' metodu altında case yazımı beklenmektedir.

• JSON body'de belirtilen data tiplerine göre metod yazımı beklenmektedir.

• Çalışma tamamlandıktan sonra çalışma yapılan collection github'a versiyon kontrolü ile push edilmesi beklenmektedir.

Script'te bulunan her request için url, method, body, headers bilgileri bulunmalı.


1-) Post metodu ile request gönderilip dönen cevaba göre;

	• Response Code(status = 200),

	• Response Time(Response Time 500 ms altında olduğu gösterilmeli.)

	• Response Key

	• Response Key Type

 kontrollerinin yapılması. 

2-) Post metodu ile request'te gönderilen body altında bulunan value'lar "" şeklinde set edilir. Daha sonra name key'i manipüle edilip value'su undefined set edilerek request gönderilmeli. Dönen cevaba göre;

	• Response Code(status = 400),
	
	• Error'daki key'ler,
	
	• Validation Error'daki key'ler,
	
	• Validation Error'da bulunan mesajın value'sunun boş olmadığı,
	
	• Validation Error'da bulunan hata kodunu yakalama
	
kontrollerinin yapılması.


3-) Get metodu ile request gönderilip dönen cevaba göre rastgele bir object seçilip 

	• Response Code(status = 200),
	
	• Response Keys,
	
	• Response Key Type
	
 kontrollerinin yapılması. 


4-) Get metodu ile request gönderilip dönen cevaba göre;

	• Response Code(status = 200),
	
	• Boş liste
	
 kontrollerinin yapılması.

5-) Post metodundan dönen Id ile put metodunun path'ini oluşturun ve put request'i atınız. Dönen cevaba göre; 

	• Response Code(status = 200),
	
	• Response body'de bulunan text mesajını doğrulama
	
kontrollerinin yapılması. 

6-) Put metodu ile random bir guid oluşturup request atınız. Body 'null' olarak gönderilmeli. (Guid için postman dynamic variable kullanın). Dönen cevaba göre;

	• Response Code(status = 405),
	
	• Error'daki key'ler,
	
	• Validation Error'daki key'ler,
	
	• Validation Error'da bulunan mesaj key value'sunun boş olmadığı,
	
	• Validation Error'da bulunan hata kodunu yakalama
	
kontrollerinin yapılması. 

7-) Post metodundan dönen Id ile delete metodunun path'ini oluşturun ve delete request'i atınız. Dönen cevaba göre; 

	• Response Code(status = 200),
	
	• Response body'de bulunan text mesajını doğrulama,
	
kontrollerinin yapılması. 

8-) Delete metodu ile random bir guid oluşturup request atınız. (Guid için postman dynamic variable kullanın). Dönen cevaba göre;

	• Response Code(status = 400)
	
	• Error'daki key'ler,
	
	• Error'daki key'ler,
	
	• Error'da bulunan mesaj key value'sunun boş olmadığı,
	
	• Error'da bulunan hata kodunu yakalama
	
kontrollerinin yapılması. 
