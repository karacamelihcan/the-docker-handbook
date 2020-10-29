# The Docker Handbook
https://www.freecodecamp.org/news/the-docker-handbook/

![](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Images/docker-handbook-github.png)

Konteynerleştirme kavramının tarihçesi oldukça eskiye dayanmasına rağmen 2013 yılında Docker Motoru'nun ortaya çıkışı, uygulamalarınızı konteyner haline getirmeyi çok daha kolay hale getirmiştir.

[Stack Overflow Developer Survey - 2020](https://insights.stackoverflow.com/survey/2020#overview) 'e göre  Docker, [en çok istenilen birinci ](https://insights.stackoverflow.com/survey/2020#technology-most-loved-dreaded-and-wanted-platforms-wanted5), [en çok sevilen ikinci](https://insights.stackoverflow.com/survey/2020#technology-most-loved-dreaded-and-wanted-platforms-loved5), ve hatta [en popüler üçüncü](https://insights.stackoverflow.com/survey/2020#technology-platforms) platform olma başarısını göstermiştir.

Her ne kadar fazlasıyla talep görse de, Docker'a yeni başlamak biraz korkutucu görünebilir. Dolayısıyla bu makalede, Konteynerleştirme ile alakalı her şeyi başlangıç seviyesinden orta seviyeye ilerleyecek şekilde öğrenmiş olacağız. Bütün makaleyi bitirdikten sonra, şunları yapabilmelisiniz:

-   (Neredeyse) her uygulamayı konteynerleştirmeli
-  Docker Hub 'a özel Docker görüntüleri yükleyebilmeli
-  Docker Compose aracını kullanarak birden fazla konteyner ile çalışabilmelisiniz.

### Ön Koşullar

-   Linux Terminal tecrübesi
-   JavaScript tecrübesi (İleriki projelerden bazıları JavaScript ile gerçekleştirilecektir)

### Kaynak Kodları
Örnek projelerin kodlarına şu repository'den ulaşabilirsiniz: 

[karacamelihcan/the-docker-handbook](https://github.com/karacamelihcan/the-docker-handbook)

### Kitabın İçeriği
-   [Konteynerleştirme ve Docker 'a Giriş](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/01.Konteynerle%C5%9Ftirme%20ve%20Docker'a%20Giri%C5%9F.md)
    -   [Sanal Makineler vs Konteynerler](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/02.Sanal%20Makineler%20vs%20Konteynerler.md)
-   [Docker'ı Yükleme](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/03.Docker'%C4%B1%20Y%C3%BCklemek.md)
-   [Docker'da Hello World](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/04.Docker'da%20Merhaba%20D%C3%BCnya.md)
    -   [Docker Mimarisi](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/05.Docker%20Mimarisi.md)
    -   [Görüntüler ve Konteynerler](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/06.G%C3%B6r%C3%BCnt%C3%BCler%20ve%20Konteynerler.md)
    -   [Kayıtlar](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/07.Kay%C4%B1tlar.md)
    -   [Bütün Resim](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/08.B%C3%BCt%C3%BCn%20Resim.md)
-   [Konteyner Manipülasyonu](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/09.Konteyner%20Manip%C3%BClasyonu.md)
    -   [Konteynerleri Çalıştırma](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/10.Konteynerleri%20%C3%87al%C4%B1%C5%9Ft%C4%B1rmak.md)
    -   [Konteynerleri Listeleme](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/11.Konteynerleri%20Listeleme.md)
    -   [Konteynerleri Yeniden Başlatma](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/12.Konteynerleri%20Yeniden%20Ba%C5%9Flatma.md)
    -   [Sarkan Konteynerleri Temizleme](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/13.Sarkan%20Konteynerleri%20Temizleme.md)
    -   [Etkileşimli Modda Konteynerleri Çalıştırma](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/14.Etkile%C5%9Fimli%20Modda%20Konteynerleri%20%C3%87al%C4%B1%C5%9Ft%C4%B1rma.md)
    -   [Çalıştırılabilir Görüntüleri Kullanarak Konteynerleri Oluşturma](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/15.%C3%87al%C4%B1%C5%9Ft%C4%B1r%C4%B1labilir%20G%C3%B6r%C3%BCnt%C3%BCleri%20Kullanarak%20Konteynerleri%20Olu%C5%9Fturma.md)
    -   [Detached Modda Konteynerleri Çalıştırma](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/16.Detached%20Modda%20Konteynerleri%20%C3%87al%C4%B1%C5%9Ft%C4%B1rma.md)
    -   [Çalışan Bir Konteyner içinde Komutları Çalıştırma](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/17.%C3%87al%C4%B1%C5%9Fan%20Bir%20Konteyner%20i%C3%A7inde%20Komutlar%C4%B1%20%C3%87al%C4%B1%C5%9Ft%C4%B1rma.md)
    -   [Çalışan Bir Konteyner içinde Kabuğu Başlatma](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/18.%C3%87al%C4%B1%C5%9Fan%20Bir%20Konteyner%20%C4%B0%C3%A7inde%20Kabu%C4%9Fu%20Ba%C5%9Flatma.md)
    -   [Çalışan Bir Konteyner'den Loglara Erişmek](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/19.%C3%87al%C4%B1%C5%9Fan%20Bir%20Konteynerden%20Loglara%20Eri%C5%9Fmek.md)
    -   [Çalışan Bir Konteyner'i Durdurma yada Öldürme](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/20.%C3%87al%C4%B1%C5%9Fan%20Bir%20Konteyneri%20Durdurma%20yada%20%C3%96ld%C3%BCrme.md)
    -   [Portları Eşleştirme](https://github.com/karacamelihcan/the-docker-handbook/blob/main/Sections/21.Portlar%C4%B1%20E%C5%9Fle%C5%9Ftirme.md)
-   [Konteyner İzolasyonunun Gösterilmesi](https://www.freecodecamp.org/news/the-docker-handbook/#demonstration-of-container-isolation)
-   [Özel Görüntüler Oluşturma](https://www.freecodecamp.org/news/the-docker-handbook/#creating-custom-images)
    -   [Görüntü Oluşturmanın Temelleri](https://www.freecodecamp.org/news/the-docker-handbook/#image-creation-basics)
    -   [Yürütülebilir Bir Görüntü Oluşturma](https://www.freecodecamp.org/news/the-docker-handbook/#creating-an-executable-image)
    -   [Ekspres Bir Uygulamayı Konteynerleştirme](https://www.freecodecamp.org/news/the-docker-handbook/#containerizing-an-express-application)
    -   [Hacimler ile Çalışma ](https://www.freecodecamp.org/news/the-docker-handbook/#working-with-volumes)
    -   [Çok Aşamalı Yapılar](https://www.freecodecamp.org/news/the-docker-handbook/#multi-staged-builds)
    -   [Yerleşik Görüntüleri Docker Hub'a Yükleme](https://www.freecodecamp.org/news/the-docker-handbook/#uploading-built-images-to-docker-hub)
-   [Docker Compose Kullanarak Birden Fazla Konteyner ile Çalışmak ](https://www.freecodecamp.org/news/the-docker-handbook/#working-with-multi-container-applications-using-docker-compose)
    -   [Compose Temelleri](https://www.freecodecamp.org/news/the-docker-handbook/#compose-basics)
    -   [Listeleme Hizmetleri](https://www.freecodecamp.org/news/the-docker-handbook/#listing-services)
    -   [Çalışan Bir Hizmet İçinde Komutları Yürütme](https://www.freecodecamp.org/news/the-docker-handbook/#executing-commands-inside-a-running-service)
    -   [Shell'i Çalışan Bir Hizmet İçinde Başlatma](https://www.freecodecamp.org/news/the-docker-handbook/#starting-shell-inside-a-running-service)
    -   [Çalışan Bir Hizmetten Loglara Erişmek](https://www.freecodecamp.org/news/the-docker-handbook/#accessing-logs-from-a-running-service)
    -   [Çalışan Hizmetleri Durdurma](https://www.freecodecamp.org/news/the-docker-handbook/#stopping-running-services)
    -   [Full-Stack Uygulama Oluşturmak](https://www.freecodecamp.org/news/the-docker-handbook/#composing-a-full-stack-application)
-   [Son](https://www.freecodecamp.org/news/the-docker-handbook/#conclusion)
