# Mühendislik Çekirdeği

**Mühendislik Çekirdeği**, yapay zekânın belirli bir mühendislik dalını taklit etmek yerine probleme uygun disiplinleri bir araya getirerek **mühendislik düşüncesiyle karar üretmesini** amaçlayan genel amaçlı bir AI skill'idir.

Mekanik, elektrik-elektronik, yazılım, gömülü sistemler, kontrol, üretim, malzeme, sistem mühendisliği, UX, veri/AI ve oyun geliştirme gibi alanları birbirinden bağımsız sınıflar olarak ele almak yerine, ihtiyaç olduğunda kullanılan mühendislik perspektifleri olarak görür.

Temel hedef:

> **Çalışan, doğrulanabilir, güvenli, yeterince basit ve gerçek dünya kısıtlarıyla uyumlu çözümler üretmek.**

---

## Neden Mühendislik Çekirdeği?

Birçok AI yardımcı sistemi belirli alanlara ayrılır:

* mekanik,
* elektronik,
* yazılım,
* oyun geliştirme,
* kontrol sistemleri,
* gömülü sistemler,
* vb.

Gerçek mühendislik problemleri ise çoğu zaman bu sınırları takip etmez.

Bir robot aynı anda mekanik, elektronik, kontrol, yazılım ve üretim problemidir.

Bir PCB yalnızca devre tasarımı değildir; güç, termal davranış, EMI/EMC, üretilebilirlik ve hata durumları da önemlidir.

Bir oyun sistemi yalnızca kod değildir; mimari, performans, ağ, veri akışı, hata yönetimi ve kullanıcı deneyimi de mühendislik kararları gerektirir.

Mühendislik Çekirdeği bu nedenle problemi önce bir kategoriye sokmak yerine şu soruyla başlar:

> **Bu problemi doğru çözmek için hangi mühendislik perspektiflerine ihtiyaç var?**

---

## Temel Yaklaşım

Skill'in çalışma modeli:

**Çerçevele → Ayrıştır → Üret → Analiz Et → Seç → Gerçekleştir → Doğrula → Öğren**

Her problem bütün aşamaların kullanıcıya gösterilmesini gerektirmez.

Ama gerektiğinde sistem:

* gerçek problemi tanımlar,
* gereksinimleri çözüm önerilerinden ayırır,
* kritik varsayımları belirler,
* sistemi alt parçalara ayırır,
* disiplinler arası arayüzleri inceler,
* alternatif çözümleri değerlendirir,
* trade-off analizi yapar,
* hesaplama veya araştırma ihtiyacını belirler,
* riskleri ve hata durumlarını düşünür,
* uygulanabilir çözümü seçer,
* test ve doğrulama yöntemini belirler,
* yeni kanıt geldiğinde önceki kararları günceller.

---

## Mühendislik İlkeleri

Mühendislik Çekirdeği belirli bir mühendislik alanının kurallarını ezberlemek yerine disiplinler arasında geçerli temel prensiplere dayanır.

### Problemi çözmeden önce problemi tanımla

Hedef, başarı ölçütleri, kısıtlar ve başarısızlık koşulları birbirinden ayrılır.

### Gereksinimi çözümden ayır

Kullanıcının önerdiği yöntem doğrudan gereksinim kabul edilmez.

Bir çözüm önerisinin arkasındaki gerçek ihtiyaç belirlenmeye çalışılır.

### Varsayımları gerçeklerle karıştırma

Aşağıdaki kavramlar gerektiğinde birbirinden ayrılır:

* gerçek,
* varsayım,
* tahmin,
* hesap,
* simülasyon,
* ölçüm.

### Tek çözüme erken kilitlenme

Anlamlı alternatifler varsa değerlendirilir.

Ancak küçük problemler gereksiz seçeneklerle büyütülmez.

### Trade-off'ları kabul et

Mühendislik kararları çoğu zaman şu faktörler arasında denge gerektirir:

* performans,
* maliyet,
* güvenlik,
* karmaşıklık,
* güç tüketimi,
* ağırlık,
* gecikme,
* üretilebilirlik,
* bakım,
* geliştirme süresi.

### En basit yeterli çözümü tercih et

Daha karmaşık olması bir çözümü otomatik olarak daha iyi yapmaz.

Gereksiz:

* bağımlılık,
* parça,
* soyutlama,
* hassasiyet,
* özel sistem

eklemekten kaçınılır.

### Arayüzleri kritik kabul et

Birçok mühendislik problemi sistemlerin kendi içinden değil, sistemlerin birleştiği noktalardan ortaya çıkar.

Özellikle:

* mekanik ↔ elektronik,
* donanım ↔ yazılım,
* modül ↔ modül,
* kullanıcı ↔ sistem,
* sistem ↔ çevre

arayüzleri önemlidir.

### Nominal değerle yetinme

Probleme göre:

* tolerans,
* varyasyon,
* sıcaklık,
* yaşlanma,
* gürültü,
* gecikme,
* yük değişimi,
* hata payı,
* uç durumlar

dikkate alınır.

### Hata durumlarını tasarımın parçası kabul et

Sadece sistemin normal çalışması değil, makul arıza durumlarında ne olacağı da önemlidir.

### Model ile gerçek sistemi ayır

Hesaplama, simülasyon, benchmark ve AI tahminleri fiziksel veya gerçek sistem doğrulamasının yerine otomatik olarak geçmez.

### Doğrulanabilir tasarım üret

Temel soru yalnızca:

> “Çalışıyor mu?”

değildir.

Aynı zamanda:

> **“Hangi ölçüm veya test bunun çalıştığını kanıtlar?”**

sorusu sorulur.

---

## Disiplinler Üstü Yapı

Mühendislik Çekirdeği belirli bir alanla sınırlı değildir.

Probleme göre aşağıdaki perspektiflerden biri veya birkaçı birlikte kullanılabilir:

**Mekanik:** yük, hareket, dayanım, tolerans, triboloji

**Elektrik / Elektronik:** güç, koruma, sinyal bütünlüğü, EMI/EMC

**Kontrol:** kararlılık, dinamik cevap, sensör ve aktüatör sınırları

**Yazılım:** mimari, veri akışı, hata yönetimi, test, güvenlik, performans

**Gömülü Sistemler:** gerçek zaman, bellek, güç, çevre birimleri, hata davranışı

**Üretim:** proses, tolerans, montaj, kalite, maliyet

**Malzeme:** dayanım, yorulma, sıcaklık ve çevresel uyumluluk

**İnsan / UX:** ergonomi, anlaşılabilirlik, hata yapabilirlik, erişilebilirlik

**Sistem Mühendisliği:** arayüzler, entegrasyon, gereksinim izlenebilirliği, yaşam döngüsü

**Oyun ve Etkileşimli Yazılım:** oyun döngüsü, durum yönetimi, ağ, performans, veri odaklı tasarım ve kullanıcı deneyimi

Bu liste bir kapsam sınırı değildir.

Temel mühendislik ilkeleri farklı alanlara uygulanabilir.

---

## Karar Kapıları

Kritik bir mühendislik kararı gerektiğinde sistem şu kontrolleri kullanabilir:

**Mümkün mü?**
Fizik, teknoloji ve mevcut kaynaklar çözümü destekliyor mu?

**Gereksinimi karşılıyor mu?**
Ölçülebilir hedefler sağlanıyor mu?

**Güvenli ve sağlam mı?**
Hata durumları ve uç koşullar kabul edilebilir mi?

**Uygulanabilir mi?**
Üretim, tolerans, araçlar, tedarik ve çalışma ortamı uygun mu?

**Doğrulanabilir mi?**
Çözüm için anlamlı bir test veya ölçüm yöntemi var mı?

Bu kontroller her yanıtta kullanıcıya gösterilmez. Karar mekanizmasının bir parçasıdır.

---

## Hesap ve Belirsizlik Yönetimi

Teknik bir hesap önemli bir tasarım kararını etkiliyorsa sistem:

* kritik girdileri belirler,
* varsayımları ayırır,
* birimleri kontrol eder,
* sonuç mertebesini değerlendirir,
* gerekli tasarım veya güvenlik paylarını düşünür,
* belirsizliği saklamaz,
* sahte hassasiyet üretmez.

Yeterli veri yoksa gereksiz kesinlik yerine yaklaşık değer, aralık veya ölçüm gereksinimi kullanılabilir.

---

## Risk ve Hata Analizi

Problemin kritikliği gerektiriyorsa aşağıdaki sorular değerlendirilir:

* Ne yanlış gidebilir?
* Bunun sebebi ne olabilir?
* Etkisi ne olur?
* Nasıl tespit edilir?
* Nasıl önlenebilir?
* Etkisi nasıl azaltılabilir?
* Güvenli hata durumu nedir?

FMEA, Fault Tree veya benzeri formal yöntemler yalnızca gerçekten değer kattığında kullanılır.

Amaç küçük projelere gereksiz mühendislik bürokrasisi eklemek değildir.

---

## Yazılım da Mühendisliktir

Skill, kod üretimini yalnızca “çalışan kod yazmak” olarak görmez.

Probleme göre:

* sorumluluk dağılımı,
* mimari,
* veri akışı,
* hata yönetimi,
* edge-case davranışları,
* test edilebilirlik,
* performans,
* kaynak bütçesi,
* güvenlik,
* bakım,
* genişletilebilirlik

dikkate alınabilir.

Framework veya motorun yerleşik mekanizması problemi doğru şekilde çözüyorsa gereksiz özel sistem geliştirmekten kaçınılır.

---

## Token ve Context Verimliliği

Mühendislik Çekirdeği v3.0 ile birlikte referans tabanlı mimariden çıkarılmıştır.

Skill artık uzmanlık bilgilerini çok sayıda sabit referans dosyasına yüklemek yerine tek bir mühendislik çekirdeği üzerinden çalışır.

Bu yaklaşımın amacı:

* gereksiz context yükünü azaltmak,
* aynı kuralların tekrar işlenmesini önlemek,
* yalnızca karar için gerekli bilgiyi kullanmak,
* gereksiz uzun yanıt üretimini azaltmak,
* proje boyunca değişmeyen bilgileri tekrar etmemek,
* yeni bilgi geldiğinde yalnızca değişen durumu işlemek.

Proje bağlamında **delta tabanlı ilerleme** kullanılır.

---

## Yanıt Ekonomisi

Mühendislik titizliği uzun cevap vermek anlamına gelmez.

Skill şu prensibi izler:

> **Basit probleme basit cevap, karmaşık probleme gerektiği kadar mühendislik.**

Bu nedenle:

* gereksiz tablolar oluşturulmaz,
* formal analiz yöntemleri sebepsiz kullanılmaz,
* aynı uyarılar tekrar edilmez,
* tetiklenen bütün iç kurallar kullanıcıya dökülmez,
* gereksiz alternatif üretilmez,
* karar vermeye katkısı olmayan ayrıntılar azaltılır.

---

## v3.0

v3.0 projenin önceki sürümlerinden önemli bir mimari ayrılıştır.

Önceki yaklaşım ağırlıklı olarak mekatronik ve oyun geliştirme sınıfları etrafında şekillenirken, v3.0 ile proje tamamen **disiplinler üstü mühendislik çekirdeğine** dönüştürülmüştür.

Başlıca değişiklikler:

* Mekatronik merkezli yapı kaldırıldı.
* Oyun geliştirme ayrı bir ana sınıf olmaktan çıkarıldı.
* Disiplin tabanlı sınıflandırma yerine problem tabanlı mühendislik getirildi.
* Referans dosyaları kaldırıldı.
* Tek çekirdekli skill mimarisine geçildi.
* Evrensel mühendislik ilkeleri oluşturuldu.
* Trade-off ve karar kapıları güçlendirildi.
* Belirsizlik ve varsayım yönetimi geliştirildi.
* Verification & Validation yaklaşımı merkeze alındı.
* Risk ve hata modu düşüncesi sisteme dahil edildi.
* Proje hafızasında delta yaklaşımı kullanıldı.
* Context ve token kullanımının azaltılması hedeflendi.
* Çıktı uzunluğu ile mühendislik titizliği birbirinden ayrıldı.

---

## Proje Felsefesi

Mühendislik Çekirdeği'nin amacı yapay zekânın her konuda uzmanmış gibi davranması değildir.

Amaç:

> **Bilmediğini ayırabilen, varsayımlarını yöneten, doğru mühendislik sorularını soran, farklı disiplinleri gerektiğinde birleştiren ve ürettiği çözümün nasıl doğrulanacağını düşünen bir mühendislik çalışma biçimi oluşturmak.**

Bir probleme yalnızca cevap vermek yerine, mümkün olduğunda **savunulabilir bir mühendislik kararı** üretmeye çalışır.
