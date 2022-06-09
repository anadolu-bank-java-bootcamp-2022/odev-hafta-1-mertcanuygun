# Liskov Substitude Principle

![LSP](https://deviq.com/static/1d86bcc5f3ee320dad22bc8a9e730308/066f9/liskov-substitution-400x400.jpg)

## Ne?
Barba Liskov tarafından geliştirilen bu SOLID prensibinin tanımı en basit şekilde alt sınıflardan oluşturulan nesnelerin üst sınıfların nesneleriyle yer değiştirdiklerinde aynı davranışı göstermek zorunda olmalarıdır. Bu durum, alt sınıf nesnelerinin üst sınıfın nesneleri gibi davranmalarını gerektirir.

## Neden?
LSP'de amaç alt sınıflarımızın nesnelerinin üst sınıfımızın nesneleri ile aynı şekilde davranmasını sağlamaktır. Bu sayede iyi bir kalıtım hiyerarşisi modellenebilir. Aynı zamanda başka bir SOLID prensibi olan **Open/Closed Principle**'a uymayan model hiyerarşilerini önlemiş oluruz. Haliyle dolaylı yoldan Open/Closed prensibi otomatik olarak sağlanmış olacaktır.

## Nasıl?
Bu prensibin nasıl uygulanacağını örnek üzerinden açıklamak daha doğru olacaktır. Çünkü uygulaması mantıksal bir kurgulama ile mümkün. Fiziki bir yol haritası çıkarmanın yolu yok. Kuş adında bir ata sınıfımız olduğunu ve içinde uçmak isimli bir method barındırdığını düşünelim. Bu ata sınıf penguen ve güvercin isimli iki alt sınıfa kalıtım vermiş olsun. Burada uçmak methodu güvercin sınıfı için doğru bir özellik iken penguen sınıfı için yanlış olacaktır. Çünkü penguenler kuş olmalarına rağmen uçamazlar. Böylece ata sınıf ile alt sınıfların aralarında yer değiştirmeleri durumunda LSP ihlal edilmiş olacaktır.

Gerçek hayattan örnek olarak ise; Komşunuzun evcil ördeğini bayatlamış Ekmek ile beslediniz ve öldü. Onu bir oyuncak ördekle değiştirmeye karar verdin. Ve sonucunda komşunuz bu durumdan mutlu değil. Çünkü iki nesne birbirinin yerine kullanılabilir değildir.
