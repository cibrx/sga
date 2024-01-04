# SGA cheatsheet

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
- Varsayılan kullanıcı adları ve domainlerin değiştirilmesi: 
  SSH gibi servisler şifrelemelerini gerçekleştirirken bu değerleri referans aldığından, varsayılan haliyle bırakmamamız önemlidir.
- Alt ağlara bölme:
  Ağların alt ağlar olacak şekilde daha küçük parçalara bölünmesi erişimi kısıtlayacağından güvenliğe katkı sağlayacaktır. Benzer amaçla kullanılan VLAN da bu konuda tercih edilebilir.
     
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

### Ağ cihazlarının fiziksel güvenliği nasıl sağlanır?
<super>Ağ güvenliğinin yazılımsal olarak güvenli tutulmasının yanında, cihazların fiziksel olarak korunması da oldukça önemlidir.</super>
- Güvenli Konum: Ağ cihazları güvenli bir yerde, yetkisiz erişimden uzakta bulunmalıdır.
- Erişim Kontrolleri: Kapılar, kilitler ve erişim kontrol sistemleri kullanarak sadece yetkili kişilerin girebilmesini sağlayın.
- Güvenlik Kameraları ve Alarm Sistemleri: Fiziksel güvenlik durumunu izlemek için güvenlik kameraları ve alarm sistemleri kullanın.
- Çevresel Kontroller: Sıcaklık, nem gibi çevresel faktörleri izleyerek cihazları koruyun.
- Kilitli Kabinetler: Ağ ekipmanlarını kilitli kabinetler içinde saklayarak fiziksel erişimi sınırlayın.
- Eğitim ve Bilgilendirme: Personeli güvenlik prosedürleri konusunda eğitin ve bilgilendirin.
### Sezar Şifreleme Nedir?
> Sezar şifrelemesi, basit bir şifreleme yöntemidir ve adını Roma İmparatoru Sezar'dan almıştır. Temel çalışma prensibi, bir metni belirli bir sayıda yer değiştirme ile şifrelemektir.
<super>Sezar şifrelemesinin temel çalışma adımları:</super>
- Anahtar Belirleme:
        - Sezar şifrelemesinde kullanılan anahtar, kaç yer kaydırma yapılacağını belirler. Bu anahtar genellikle bir sayıdır.

- Metni Şifreleme:
        - Her harfi belirlenen anahtar kadar kaydırarak şifreleme işlemi gerçekleştirilir. Örneğin, anahtar 3 ise 'A' harfi 'D' haline gelir.

- Şifrelenmiş Metni Oluşturma:
        - Tüm harfler bu kaydırma işlemine tabi tutularak şifrelenmiş metin oluşturulur.

Örneğin 'HELLO' metnini 3 anahtarıyla şifrelediğimizde şifreleme adımları şu şekilde olacaktır:

- 'H' harfi 3 birim kaydırılır ve 'K' olur.
- 'E' harfi 3 birim kaydırılır ve 'H' olur.
- 'L' harfi 3 birim kaydırılır ve 'O' olur.
- 'L' harfi 3 birim kaydırılır ve 'O' olur.
- 'O' harfi 3 birim kaydırılır ve 'R' olur.

<strong>Şifrelenmiş metin: "KHOOB"</strong>

### SSH Yapılandırılmasında key oluşturulurken hangi algoritma kullanılır?
> SSH, kullanıcıların sunucularını veya cihazlarını internet üzerinden kontrol etmelerine olanak sağlayan bir protokoldür. SSH bağlantılarında güvenliği sağlayan bir şifreleme tekniği bulunur. Bu şifreleme *RSA* algoritması kullanılarak gerçekleştirilir.


RSA, yaygın olarak kullanılan bir asimetrik şifreleme algoritmasıdır. Bu algoritmada biri açık diğeri ise özel olmak üzere 2 anahtar bulunur ve şifrelemelerde bunlardan yararlanılır.
### Hash ve Şifreleme arasındaki farklar nedir?
> Şifreleme ve hashleme arasındaki ana fark, birinin geri döndürülebilir olması, diğerinin ise gerçekleştirildikten sonra geri alınamamasıdır.


Şifreleme, bir veriye veya metne erişilebilmesi için bir şifrenin gerekli kılınmasıdır. Böylelikle veriye sadece erişmesi gereken kişiler erişir. Böylelikle verilerin bütünlüğü ve güvenliği sağlanmış olur.

Hashleme ise benzer bir amaçla yapılır, verilerin bütünlüğünü sağlar. Ancak hashleme tek yönlüdür, hashlenen bir veri tekrardan orijinal haline çevrilemez. Böylece veriler güvenli şekilde tutulmuş ve erişimlerden korunmuş olur.

### Veritabanı Nedir?
> Veritabanları; çeşitli türden verilerin depolanmasını ve gerektiğinde erişilmesi işlemini kolaylaştırmak için geliştirilmiş sistemlerdir.


Veritabanları depoladıkları verileri ilişkilendirmek, hızlı sorgular gerçekleştirmek gibi çeşitli amaçlarda sürekli geliştirilmektedir. Günümüzde oldukça fazla çeşidi bulunan veritabanları, bazı avantajlar ve özelliklerle öne çıkarlar. 

Veritabanları üç kısımda incelenir: 

- İlişkisel Veritabanları (RDBMS - SQL): Bu tür veritabanlarında her bir verinin içerdiği özellikler ilişkilendirilerek saklanır. Sorgular gerçekleştirilirken de bu durumdan yararlanılır. İlişkisel veritabanlarında satırlar her farklı verileri, sütunlar ise her bir verinin içerdiği ayrı alanları temsil eder. Ayrıca ilişkisel veritabanlarında sorgulama gerçekleştirmek için geliştirilmiş diller(query language) vardır.
- Nesne Odaklı Veritabanları(OODBMS): Veritabanlarındaki verilerin, programlama dillerindeki nesne(object) kavramıyla temsil edildiği sistemlere nesne odaklı veritabanı adı verilir. Nesne odaklı veritabanlarına çok rastlanmasa da diğer veritabanı çeşitlerini benzer şekilde kullanmak için geliştirilmiş yazılımlar sıklıkla kullanılmaktadır.
- İlişkisel Olmayan Veritabanları (NRDBMS - NoSQL): Veriler arasında ilişki kurulması yerine verilerin direkt olarak depolanması amacıyla geliştirilmiş veritabanlarıdır. Sorgu dilleri yerine direkt olarak içerilen verilerle sorgulamalar yapılır. Farklı ve değişken veri tipleri için uyumlulardır ve geliştiricilere kolaylık sağlarlar. Buna rağmen büyük verilerde sorgulamaların zorluğu ve yetersizliği, kullanıcılar için sorun teşkil edebilir. 

### SQL Nedir?
> Structured Query Language(SQL), ilişkisel veritabanlarıyla etkileşimde bulunmak için oluşturulmuş bir dildir. Veritabanındaki tablo işlemleri, verilerin eklenmesi/silinmesi/düzenlenmesi, sorgulama gerçekleştirilerek verilere erişilmesi SQL aracılığıyla sağlanır.
### Verilerin Yapılandırılması:

<strong>Yapılandırılmış Veri</strong>
> Yapılandırılmış veri, belirli bir düzen içinde organize edilmiş ve genellikle veritabanlarında depolanan veriyi temsil eder. Veritabanları, yapılandırılmış veriyi tablolar, sütunlar ve satırlar şeklinde düzenleyerek bilgiyi düzenli bir şekilde saklamak ve erişmek için kullanılır. Bu düzen, veri üzerinde etkili sorgulama, güncelleme ve analiz işlemleri gerçekleştirmeyi sağlar. Yapılandırılmış veri, bilgi yönetiminde düzeni ve tutarlılığı artırmak için önemlidir.



<strong>Yapılandırılmamış Veri</strong>
> Bu konuda herhangi bir uygulama yerine getirilmemiş, saf şekilde veriyi depolama şekline ise yapılandırılmamış veri adı verilir.

# SGA - Uygulama Kısmı

### SSH ağ sıkılaştırılması
[link](https://github.com/LegendMan46/sga/blob/main/README.md)
