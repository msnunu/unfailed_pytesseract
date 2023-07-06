# unfailed_pytesseract
Github'a başarısız olunmuş bir fikir atılır mı derseniz eğer, ben attım valla. Hevesliydim bu mini iş için ama olduramadım hiçbir şekilde. İleride geri dönüp çözebilmek dileğiyle :)
#### Amacım neydi, nereden esti bu fikir?
YTÜ'23 mezuniyeti için Erhan Öztürk'ün hazırlamış olduğu tasarım şöyleydi:

![ytü23](https://github.com/msnunu/unfailed_pytesseract/assets/124269047/1ca156bb-a88b-430b-8a9f-126f49a8d045)

Çok tatlı bir tasarım tabii, sosyal medyadan dönüşler de güzeldi bence. Ama..
Burada ismimizi bulmak için mezuniyet günümüzde gözlerimizi incitmeyelim dedim, ocr gibi konuları okuyup araştırmaya başladım.

#### Nasıl yapmaya çalıştım?
Yukarıdaki tasarımın yüksek çözünürlüklü hali elimde olmadığından ve kalp şeklinin bir tık zorluk çıkaracağını düşünerek önce kendi resmimi oluşturmalıydım.
1. list_to_image : Kendi görselimi oluşturmak için yazdığım kodları içeren notebook.
   Burada Faker kütüphanesini kullanarak 500 kişilik bir mezuniyet_listesi oluşturdum. Daha sonra for döngüsü ve if kontrolleri ile yığılma olmadan Pillow kütüphanesinden ImageNew,ImageDraw gibi paketlerinden faydalandım.
   Sonuç olarak çıktı bu şekildeydi:
   
   ![direct_textoimage](https://github.com/msnunu/unfailed_pytesseract/assets/124269047/808e223b-0390-4dff-bd77-fa3221dd1509)

   Tabii bu çıktı diğerinin yanında çok çirkin kaldı. Ama şu an estetik kısma takılmıyorum, Adobe gibi programlardan resim çıktısı oluşturuladabilir.
   Asıl amacım bu resmi Pytesseract aracılığı ile text'e çevirip, kullanıcıdan ismini alıp işaretleyerek yeni bir resim çıktısı oluşturmasıydı.
   Maalesef başarısız oldu bu.

   👀Ayrıca neden text'ten image'a, image'tan text'e dönüştürüyorsun derseniz; senaryoyu sanki mezuniyet günü resmi çekmiş ve ismimizi bulmaya çalışmışız gibi düşünün.
   Ben elimde yan yana sıralı isimlerden oluşan bir text'in resmi olmadığı için ve bunu Word vs. değil de Python'da yapmak istediğim için bu şekilde yaptım.
   Asıl pytesseract kullanılan notebooku ve hatalı sonuçları en kısa zamanda yükleyeceğim, şu an o notebookların içi çok karışık😂

