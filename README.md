# IremGulten_SOLID
Bu proje SOLID prensiplerinin açıklanmasını ve SRP, OCP prensiplerinin örnek uygulamasını içermektedir.<br>

#1) S -> Single Responsibility Principle
Single Responsibility prensibi,temelde her bir nesnenin sadece tek bir işi yapması gerektiğini vurgulamaktadır. Eğer ben üzerinde çalıştığım projenin içindeki herhangi bir nesnede yapmam gereken değişiklik için birden fazla sebep buluyorsam bu prensibe uymuyorum demektir.

#2) O -> Open-Closed Principle
Open-Closed prensibi, bir nesnenin gelişime AÇIK fakat değişime KAPALI olduğunu vurgulamaktadır. Aslında aktarılmak istenen nesnelerin temel özelliklerinin değiştirilmeden nesneye ekleme yapılabiliyor olması gerektiğidir. Eğer ben üzerinde çalıştığım bir projeye yeni bir özellik eklemek istediğimde mevcutta bulunan bir nesneyi değiştirmek zorundaysam bu prensibe uymuyorum demektir. 

#3) L -> Liskov Substitution Principle
Liskov Substitution prensibi, bir sınıftan miras alan iki sınıfın birbirlerinin yerine ve üst sınıftan oluşan nesnenin yerine İSTİSNASIZ kullanılabilmesi gerektiği vurgulamaktadır. Yani, miras alarak türetilen sınıflar önce miras alındıkları nesnenin tüm özelliklerini kullanmalı, daha sonra kendi özelliklerini eklemesi gerekmektedir. Eğer ben bir sınıftan miras alan her sınıfın kendi nesnesine özel kod blokları ekliyorsam bu prensibe uymuyorum demektir.

#4) I -> Interface Segregation Principle
Interface Segregation prensibi, her nesnenin kendi amacına uygun property veya metotlar içeren interface’leri implement etmesi gerektiğini vurgulamaktadır. Yani bu prensip bizlere herhangi bir interface’e ait bir metot için tüm interface’i implement etmememiz gerektiğini ve bu gibi durumlarda interface’leri ayırmamız gerektiğini söylemektedir. Eğer ben bir interface’i implement ettiğimde bu interface’in bir metodu benim sınıfım için anlamsızsa bu prensibe uymuyorum demektir ve yapmam gereken, interface’i parçalara ayırarak sadece kullanacağım metodları bir interface’te toplamaktır.

#5) D -> Dependency Inversion Principle
Dependency Inversion prensibi, büyük sistemlerin küçük sistemlere değil, küçük sistemlerin büyük sistemlere bağlı olması gerektiğini vurgulamaktadır. <br>Bu prensibe günlük hayattan bir örnek vermek istiyorum. Örneğin telefonumun ekranı çatladı ve telefonumu tamir için servise götürdüm. Servisteki adam bana “Bu telefonun camı kırılmış sen bunu kullanamazsın artık yeni telefon alman gerekiyor…” dedi. Böyle bir durum söz konusu olamaz değil mi :) Çünkü aslında telefon cama bağımlı değil, cam telefona bağımlı. Prensimiz de bize tam olarak bunu söylemekte. Kurduğunuz sistemlerde bağımlı olunan büyük sistem ve bağımlı olan da küçük sistem olmalı.
