# Homework-1

### 1. Java’nın platform bağımsızlığını nasıl sağladığını anlatınız.(5 PUAN)

Java bir kere yaz her yerde çalışsın mottosu ile çalışıyor. C - C# gibi diller makinenin işletim 
sisteminde derlendiği için platform bağımlılardır.  Fakat Java JVM(Java Virtual Machine) üzerinden çalışmaktadır. 
Bu sayede platformdan bağımsız olarak aynı bytecode'u üretir. Bu sayede de istediğimiz platformda 
çalıştırabilmemizi sağlar. Burada dezavantaj hız olarak karşımıza çıkmaktadır. Bunun nedeni işletim 
sistemi ile birlikte Virtual Machine'in de bilgisayarın kaynaklarını kullanmasıdır.


### 2. Java neden çoklu kalıtımı desteklemez? Hangi diller bu duruma neden izin verir? (5 PUAN)
Karmaşıklığı azaltmak ve dili basitleştirmek için çoklu kalıtım desteklenmez. 

### 3. Build Tool nedir? Java ekosistemindeki toollar neler?
### 4. Collection framework içerisindeki yapıları örnekleyip açıklayınız. (20 PUAN)
### 5. Bir müşterinin, sipariş oluşturup, faturalarını kaydedebildiği ve görüntüleyebildiği bir uygulama
yazın. Final, static, overload, override, constructor, kalıtım, polimorfizim, encapsulation, List, Set,
Map kavramlarını kullanılmalıdır. Sisteme eklemeler yapabilirsiniz. Main method üzerinde
çalışması yeterlidir. SOLID prensiplerine uygun olarak yazmaya çalışınız. Kod kalitesi
puanlanacaktır, isimlendirme kurallarına dikkat ediniz. Listeleme işlemleri stream kullanılarak
yapılmalı.(70 PUAN)
• Maven projesi oluşturun.
• Maven komutlarını çalıştırıp, çıktıyı ekleyin

#### Clean
````
[INFO] Scanning for projects...
[INFO] 
[INFO] -------------------------< org.example:hwork1 >-------------------------
[INFO] Building hwork1 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-clean-plugin:2.5:clean (default-clean) @ hwork1 ---
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  0.246 s
[INFO] Finished at: 2022-06-15T22:44:53+03:00
[INFO] ------------------------------------------------------------------------
````
#### Validate
````
````
#### Compile
````
````
#### Test
````
````
#### Package
````
````
#### Verify
````
````
#### Install
````
````
#### Site
````
````
#### Deploy
````
````
• Tüm müşterileri listeleyin
• Yeni Müşteri oluşturabilen
• İçerisinde ‘C’ harfi olan müşterileri listeleyin
• Haziran ayında kayıt olan müşterilerin faturalarınının toplam tutarını listeleyin
• Sistemdeki tüm faturaları listeleyin
• Sistemdeki 1500TL üstündeki faturaları listeleyin
• Sistemdeki 1500TL üstündeki faturaları ortalamasını hesaplayın
• Sistemdeki 500TL altındaki faturalara sahip müşterilerin isimleri listeleyin
• Haziran ayını faturalarını ortalaması 750 altı olan firmalarının hangi sektörde olduğunu listeleyen
kodu yazın.

Bu dosya Patika.dev - LOGO Java & Spring Boot eğitimi dışında kullanılamaz.
Cem DIRMAN
