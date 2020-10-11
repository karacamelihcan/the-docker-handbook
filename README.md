# Docker El Kitabı
https://www.freecodecamp.org/news/the-docker-handbook/

![](https://github.com/karacamelihcan/the-docker-handbook/blob/main/docker-handbook-github.png)

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
-   [Konteynerleştirme ve Docker 'a Giriş](https://www.freecodecamp.org/news/the-docker-handbook/#introduction-to-containerization-and-docker)
    -   [Sanal Makineler vs Konteynerler](https://www.freecodecamp.org/news/the-docker-handbook/#virtual-machines-vs-containers)
-   [Docker'ı Yükleme](https://www.freecodecamp.org/news/the-docker-handbook/#installing-docker)
-   [Docker'da Hello World](https://www.freecodecamp.org/news/the-docker-handbook/#hello-world-in-docker)
    -   [Docker Mimarisi](https://www.freecodecamp.org/news/the-docker-handbook/#docker-architecture)
    -   [Görüntüler ve Konteynerler](https://www.freecodecamp.org/news/the-docker-handbook/#images-and-containers)
    -   [Kayıtlar](https://www.freecodecamp.org/news/the-docker-handbook/#registries)
    -   [Bütün Resim](https://www.freecodecamp.org/news/the-docker-handbook/#the-full-picture)
-   [Konteyner Manipülasyonu](https://www.freecodecamp.org/news/the-docker-handbook/#manipulating-containers)
    -   [Konteynerleri Çalıştırma](https://www.freecodecamp.org/news/the-docker-handbook/#running-containers)
    -   [Konteynerleri Listeleme](https://www.freecodecamp.org/news/the-docker-handbook/#listing-containers)
    -   [Konteynerleri Yeniden Başlatma](https://www.freecodecamp.org/news/the-docker-handbook/#restarting-containers)
    -   [Sarkan Konteynerleri Çalıştırma](https://www.freecodecamp.org/news/the-docker-handbook/#cleaning-up-dangling-containers)
    -   [Etkileşimli Modda Konteynerleri Çalıştırma](https://www.freecodecamp.org/news/the-docker-handbook/#running-containers-in-interactive-mode)
    -   [Çalıştırılabilir Görüntüleri Kullanarak Konteynerleri Oluşturma](https://www.freecodecamp.org/news/the-docker-handbook/#creating-containers-using-executable-images)
    -   [Ayrılmış Modda Konteynerleri Çalıştırma](https://www.freecodecamp.org/news/the-docker-handbook/#running-containers-in-detached-mode)
    -   [Çalışan Bir Konteyner içinde Komutları Çalıştırma](https://www.freecodecamp.org/news/the-docker-handbook/#executing-commands-inside-a-running-container)
    -   [Çalışan Bir Konteyner içinde Kabuğu Başlatma](https://www.freecodecamp.org/news/the-docker-handbook/#starting-shell-inside-a-running-container)
    -   [Çalışan Bir Konteyner'den Loglara Erişmek](https://www.freecodecamp.org/news/the-docker-handbook/#accessing-logs-from-a-running-container)
    -   [Çalışan Bir Konteyner'i Durdurma yada Öldürme](https://www.freecodecamp.org/news/the-docker-handbook/#stopping-or-killing-a-running-container)
    -   [Portları Eşleştirme](https://www.freecodecamp.org/news/the-docker-handbook/#mapping-ports)
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
