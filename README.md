# Görev
Projede SDET.postman_collection.json isimli dosya bulunmaktadır. Postman collection'ında bulunan API'ler için JSON formatında, Post - Get - Put - Delete metotları ile request gönderilip response'da dönen key ve key value'lara göre soruların cevapları beklenmektedir. Tek bir 'Post' metodu altında script yazımı beklenmektedir.

Collection'da bulunan request'lerle ilgili dokümanı ayrı olarak incelenmek istenirse:
https://documenter.getpostman.com/view/24419403/2s8ZDbWgPN


1-) Post metodu ile request gönderilip dönen cevaba göre;

	• Response Code(status = 200),

	• Response Time(Response Time 500 ms altında olduğu gösterilmeli.)

	• Response Key

	• Response Key Type

 kontrollerinin yapılması. 

2-) Post metodu ile request'te gönderilen body altında bulunan key'lerden name key'i manipüle edilip property value'su undefined set edilerek request gönderilmeli. Dönen cevaba göre;

	• Response Code(status = 200),
	
	• Error'daki key'ler,
	
	• Validation Error'daki key'ler,
	
	• Validation Error'da bulunan mesajın key value'sının boş olmadığı,
	
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

8-) Put metodu ile random bir guid oluşturup request atınız. (Guid için postman dynamic variable kullanın). Dönen cevaba göre;

	• Response Code(status = 400)
	
	• Error'daki key'ler,
	
	• Error'daki key'ler,
	
	• Error'da bulunan mesaj key value'sunun boş olmadığı,
	
	• Error'da bulunan hata kodunu yakalama
	
kontrollerinin yapılması. 
	
	


