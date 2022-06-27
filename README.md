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
[INFO] Scanning for projects...
[INFO] 
[INFO] -------------------------< org.example:hwork1 >-------------------------
[INFO] Building hwork1 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  0.196 s
[INFO] Finished at: 2022-06-15T23:37:07+03:00
[INFO] ------------------------------------------------------------------------
````
#### Compile
````
[INFO] -------------------------< org.example:hwork1 >-------------------------
[INFO] Building hwork1 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ hwork1 ---
[INFO] Changes detected - recompiling the module!
[WARNING] File encoding has not been set, using platform encoding UTF-8, i.e. build is platform dependent!
[INFO] Compiling 2 source files to C:\Users\asus\Documents\GitHub\homework-1-yusufceylann\target\classes
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  2.589 s
````
#### Test
````
[INFO] -------------------------< org.example:hwork1 >-------------------------
[INFO] Building hwork1 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ hwork1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory C:\Users\asus\Documents\GitHub\homework-1-yusufceylann\src\test\resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ hwork1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ hwork1 ---
[INFO] No tests to run.
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  1.566 s
[INFO] Finished at: 2022-06-15T23:38:14+03:00
[INFO] ------------------------------------------------------------------------
````
#### Package
````
[INFO] -------------------------< org.example:hwork1 >-------------------------
[INFO] Building hwork1 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ hwork1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory C:\Users\asus\Documents\GitHub\homework-1-yusufceylann\src\test\resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ hwork1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ hwork1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ hwork1 ---
[INFO] Building jar: C:\Users\asus\Documents\GitHub\homework-1-yusufceylann\target\hwork1-1.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  2.162 s
[INFO] Finished at: 2022-06-15T23:38:52+03:00
[INFO] ------------------------------------------------------------------------
````
#### Verify
````
[INFO] -------------------------< org.example:hwork1 >-------------------------
[INFO] Building hwork1 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ hwork1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory C:\Users\asus\Documents\GitHub\homework-1-yusufceylann\src\test\resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ hwork1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ hwork1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ hwork1 ---
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  1.860 s
[INFO] Finished at: 2022-06-15T23:39:19+03:00
[INFO] ------------------------------------------------------------------------
````
#### Install
````
[INFO] -------------------------< org.example:hwork1 >-------------------------
[INFO] Building hwork1 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 0 resource
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ hwork1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ hwork1 ---
[WARNING] Using platform encoding (UTF-8 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory C:\Users\asus\Documents\GitHub\homework-1-yusufceylann\src\test\resources
[INFO] 
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ hwork1 ---
[INFO] Nothing to compile - all classes are up to date
[INFO] 
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ hwork1 ---
[INFO] No tests to run.
[INFO] 
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ hwork1 ---
[INFO] 
[INFO] --- maven-install-plugin:2.4:install (default-install) @ hwork1 ---
[INFO] Installing C:\Users\asus\Documents\GitHub\homework-1-yusufceylann\target\hwork1-1.0-SNAPSHOT.jar to C:\Users\asus\.m2\repository\org\example\hwork1\1.0-SNAPSHOT\hwork1-1.0-SNAPSHOT.jar
[INFO] Installing C:\Users\asus\Documents\GitHub\homework-1-yusufceylann\pom.xml to C:\Users\asus\.m2\repository\org\example\hwork1\1.0-SNAPSHOT\hwork1-1.0-SNAPSHOT.pom
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  2.549 s
[INFO] Finished at: 2022-06-15T23:40:00+03:00
[INFO] ------------------------------------------------------------------------
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
