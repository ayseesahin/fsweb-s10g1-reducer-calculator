# Sorunu Anlamak:

1. 1 butonuna basılmasından, güncellenen değerimizin render edilmesine kadar olan uygulama adımları nelerdir?
   Her adım için kodun hangi bölümünün geçerli olduğunu listeleyin.

- Kullanıcı 1 butonuna tıkladı. Bu buton, App.js componentinde onClick eventi ile tanımlanır.
- Onclick event handler metodu ile addOne action oluşturucusunu çağırıyoruz ve burada oluşan action değerini de reducer fonksiyonuna gönderiyoruz ve total state'i 1 arttırıyoruz.
- Daha sonra ./reducer/index.js dosyasındaki reducer fonksiyonu içindeki ADD_ONE case bloğu tarafından total state güncellenir.
- App.js componenti, güncellenen total state'i alır ve yeniden render edilir.
- TotalDisplay componenti, güncellenen total state'ini gösterir. TotalDisplay total artı 1'i gösterdi.
