# SGA

### Ağ cihazlarının sıkılaştırılması nedir?
> Ağ cihazlarının sıkılaştırılması, potansiyel problemlerin ve zaafiyetlerin ortaya çıkmasını hedefleyerek güvenlik risklerinin ortadan kaldırılması aşamasıdır.<br>


<super>Bu durumun sağlanması için alınabilecek çeşitli önlemler vardır:</super>
- Gereksiz Portları Kapatma:
  Kullanılmayan portları kapatmak, potansiyel güvenlik risklerini azaltır.
- Telnet benzeri Servisleri Kapatma:
  Güvenlik açısından sıkıntılı protokol ve servislerin kapatılması ağ güvenliğini arttırmak açısından önemli etki sağlayacaktır.
- Güçlü Şifre Politikaları:
  Güçlü ve uzun şifrelerin kullanılmasının ağ sistemimizin güvenliğine katkısı oldukça büyük olabilir.
- Firewall Kuralları:
  Güvenlik Duvarının kurallarının incelenmesi, gözden geçirilmesi ve gerekirse değişimler yapılması gereklidir.
- Güncel Yazılımlar:
  Ağ sistemimizde kullandığımız yazılımların güncel tutulması, açıklar ve zaafiyetler açısından bizi korumalı tutacaktır.
- Erişim Kontrolü ve Kullanıcı Yönetimi:
  Gereksiz yetkilendirmeleri önlemek ve kullanıcıların kontrolünü sıklıkla gerçekleştirmek, ağımızın güvenliğinde önemli rol oynar.    
### Ağın güvenliğini sağlamak için hangi cihazlar kullanılmalıdır?
<super>Ağ güvenliğinin sağlanması için çeşitli cihazların kullanılması tavsiye edilir:</super>
- Firewall: Ağ trafiğini kontrol eder.
- IPS (Sızma Önleme Sistemi): Zararlı aktiviteleri algılar ve önler.
- Antivirus ve Antimalware: Zararlı yazılımları engeller.
- VPN Cihazları: Güvenli iletişim için kullanılır.
- WAF (Web Application Firewall): Web uygulamalarını korur.
- Proxy Sunucuları: İnternet trafiğini filtreler.
- Switch ve Router Güvenlik Ayarları: Güvenlik politikalarını uygular.
- Ağ İzleme ve Loglama Araçları: Anormal aktiviteleri izler.
- Authentication Servers: Kullanıcı kimlik doğrulama süreçlerini yönetir.
- NAC (Network Access Control) Cihazları: Ağ erişimini kontrol eder.

### Ağ cihazlarının fiziksel güvenkiği nasıl sağlanır?
<super>Ağ güvenliğinin yazılımsal olarak güvenli tutulmasının yanında, cihazların fiziksel olarak korunması da oldukça önemlidir.</super>
- Güvenli Konum: Ağ cihazları güvenli bir yerde, yetkisiz erişimden uzakta bulunmalıdır.
- Erişim Kontrolleri: Kapılar, kilitler ve erişim kontrol sistemleri kullanarak sadece yetkili kişilerin girebilmesini sağlayın.
- Güvenlik Kameraları ve Alarm Sistemleri: Fiziksel güvenlik durumunu izlemek için güvenlik kameraları ve alarm sistemleri kullanın.
- Çevresel Kontroller: Sıcaklık, nem gibi çevresel faktörleri izleyerek cihazları koruyun.
- Kilitli Kabinetler: Ağ ekipmanlarını kilitli kabinetler içinde saklayarak fiziksel erişimi sınırlayın.
- Eğitim ve Bilgilendirme: Personeli güvenlik prosedürleri konusunda eğitin ve bilgilendirin.
### Sezar Şifreleme nasil çalışır bir örnek veriniz 
> Sezar şifrelemesi, basit bir şifreleme yöntemidir ve adını Roma İmparatoru Sezar'dan almıştır. Temel çalışma prensibi, bir metni belirli bir sayıda yer değiştirme ile şifrelemektir.
<super>Sezar şifrelemesinin temel çalışma adımları:</super>
- Anahtar Belirleme:
        - Sezar şifrelemesinde kullanılan anahtar, kaç yer kaydırma yapılacağını belirler. Bu anahtar genellikle bir sayıdır.

- Metni Şifreleme:
        - Her harfi belirlenen anahtar kadar kaydırarak şifreleme işlemi gerçekleştirilir. Örneğin, anahtar 3 ise 'A' harfi 'D' haline gelir.

- Şifrelenmiş Metni Oluşturma:
        - Tüm harfler bu kaydırma işlemine tabi tutularak şifrelenmiş metin oluşturulur.

Örnek:

    Metin: "HELLO"
    Anahtar: 3

Şifreleme adımları:

    - 'H' harfi 3 birim kaydırılır ve 'K' olur.
    - 'E' harfi 3 birim kaydırılır ve 'H' olur.
    - 'L' harfi 3 birim kaydırılır ve 'O' olur.
    - 'L' harfi 3 birim kaydırılır ve 'O' olur.
    - 'O' harfi 3 birim kaydırılır ve 'R' olur.

<strong>Şifrelenmiş metin: "KHOOB"</strong>

### SSH yapılandirilmasinda bulunan key üretme işleminde hangi tür algoritma kullanilir?
> RSA şifreleme algoritmasi

### Hashleme ile Şifrleme arasidaki fark nedir?
> Hashleme algoritmaları geri döndürülemez bir output oluşturur. -- Şifreleme algoritmalari ise geri döndürülerbilir algoritmalar ile oluşturulur.

## DB 
### Veritabani Nedir?
> Veritabanı, düzenli bir şekilde bilgi depolayan ve erişimi sağlayan bir sistemdir. Tablolar, satırlar, sütunlar gibi temel öğeler içerir. İş ve uygulama alanlarında büyük miktarlardaki verileri organize etmek ve yönetmek için kullanılır.
### SQL Nedir?
> SQL (Structured Query Language), veritabanlarıyla iletişim kurmak için kullanılan bir dilidir. Veritabanı oluşturma, tablo işlemleri, veri ekleme, güncelleme, silme, sorgulama ve veri sıralama gibi temel görevleri gerçekleştirmek için kullanılır.
### Yapılandırılmış Veri Nedir?
> Yapılandırılmış veri, belirli bir düzen içinde organize edilmiş ve genellikle veritabanlarında depolanan veriyi temsil eder. Veritabanları, yapılandırılmış veriyi tablolar, sütunlar ve satırlar şeklinde düzenleyerek bilgiyi düzenli bir şekilde saklamak ve erişmek için kullanılır. Bu düzen, veri üzerinde etkili sorgulama, güncelleme ve analiz işlemleri gerçekleştirmeyi sağlar. Yapılandırılmış veri, bilgi yönetiminde düzeni ve tutarlılığı artırmak için önemlidir.
### 
