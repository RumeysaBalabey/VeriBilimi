# VeriBilimi
1) Json ve Dictionary arasındaki fark nedir?
* JSON, ayrıştırma veya serileştirmeye gerek kalmadan JavaScript programlarında kullanılabilir.
JavaScript nesne sabit metinlerini, dizilerini ve skaler verilerini temsil eden metin tabanlı bir yöntemdir.
JSON, okuması ve yazmasının nispeten kolay olmasının yanı sıra yazılımın ayrıştırması ve oluşturması için de kolaydır.
Genellikle, yapılandırılmış verileri seri hale getirmek ve bir ağ üzerinden (genellikle bir sunucu ile web uygulamaları
arasında) aktarmak için kullanılır.
Python collection veri tiplerinden olan dictionary yani sözlük veri
yapısı key ve value şeklinde verileri saklayabileceğimiz bir veri yapısıdır. 
Dictionary veri yapısı Json veri yapısına oldukça benzerdir.
JSON ifadelerinde her öğe arasında virgül olmalıdır. Anahtar ve değer ikilisi arasında ise iki nokta kullanılır.

- Dumps ne işe yarar?
* Dumps fonksiyonu istenilen çıktının json olup olmadığını söyler. 

- Neden encode kullanılır?(Neden data.encode.utf-8nşeklinde kullanmadık?)
* Encode UTF-8'den daha hızlı işlem yapar böylelikle daha kolay depolama yapar.

2) Json dumps nedir?
* Dumps fonksiyonu str tipinde bir değer döndürürken dump fonksiyonu hiçbir değer döndürmez.

- Json load nedir?
* load fonksiyonu sadece dosyadaki JSON verilerini Python verisine çevirir

- Json loads nedir?
* loads fonksiyonu veriyi parametre olarak alıyor

3) Docker a girdikten sonra spesific bir container hangi networkta çalışır?
* Bridge network'ta çalışır.

- Default ip nasıl bulunur?
* docker inspect -f “{{range.NetworkSettings.Networks}}{{.IPAddress}}{{end}}” ContainerID

4) Neden UTF-8 kullanıyoruz?
* Değişken kod uzunluğu, Kodlanmış bayt dizilerinin uzunluklarının açıkça belirtiliyor olması, Kendini eş zamanlama,
Çok baytlı ve tek baytlı karakterler arasındaki açık ayrım,, Geriye doğru uyumluluk özelliklerine sahiptir.


5) 192.168.0.1 nedir ve 127.00.01 ile arasındaki fark nedir?
192.168.0.1 IP adresi, ülkemizde sıklıkla kullanılan yerel IP adreslerinden biridir. Modem veya router 
yönetim arayüzüne ulaşmak için bu IP adresi kullanılmaktadır. 127.0.0.1, bilgisayarın sahip olduğu yerel IP adresi 
yani bir diğer deyişle Localhost adresidir. Bilgisayarınıza bir web sunucusu veya yazılımı kurduğunuz anda yazılım
bilgisayarınızla bu IP adresi üzerinden iletişime geçecektir.
