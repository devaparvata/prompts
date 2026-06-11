Bu klasör, belirli bir konu alanına değil; yapay zekâ çıktılarının akıl yürütme, kanıt, doğrulama, varsayım, tutarlılık ve kalite kontrol süreçlerine odaklanan meta-promptları içerir.

|Prompt|İşlev|
|---|---|
|Metabilişsel Check|Modelin kendi cevabını varsayım, eksik bilgi, tutarlılık ve aşırı yorum açısından denetlemesi|
|Chain of Evidence|Her iddiayı kanıt, kaynak, gözlem veya metin dayanağına bağlama|
|Chain of Verification|Üretilen cevabı adım adım doğrulama, hata ve zayıf halka arama|
|Tree of Thoughts|Birden fazla çözüm/yorum yolu üretip en sağlam hattı seçme|
|ReAct|Reasoning + Acting mantığıyla düşünme, arama, kontrol etme, yeniden değerlendirme|
|Varsayım Denetimi|Açık ve örtük varsayımları listeleme|
|Çıktı Kalite Denetimi|Üretilen cevabı kalite, yapı, doğruluk, kapsam ve kullanılabilirlik açısından puanlama|
|Kritik Akıl Yürütme Kontrol Listesi|Mantık hatası, genelleme, çelişki, anakronizm, kaynak zayıflığı kontrolü|


Her büyük analiz promptunun sonuna ileride şu opsiyonu ekleyebilirsin:

## Opsiyonel Kalite Kontrol

Analizi tamamladıktan sonra şu meta-denetimlerden uygun olanları uygula:

- Metabilişsel Check
- Chain of Evidence
- Chain of Verification
- Varsayım Denetimi
- Yanlış Okuma Riski Kontrolü



### Üretim sırası

**1. Chain of Evidence / CoE Super Prompt v1.0**  
Her önemli iddiayı kanıta bağlar.  
Formatı: `İddia → Kanıt → Kaynak / Gözlem → Güven Düzeyi → Eksik Bilgi`

**2. Chain of Verification / CoV Super Prompt v1.0**  
Üretilmiş cevabı doğruluk, tutarlılık, kapsam ve hata riski açısından denetler.

**3. Varsayım ve Belirsizlik Denetimi Super Prompt v1.0**  
Açık / örtük varsayımları, eksik verileri ve güven düzeylerini çıkarır.

**4. Çıktı Kalite Denetimi Super Prompt v1.0**  
Bir cevabı 100 üzerinden puanlar; kapsam, yapı, doğruluk, dil, kullanılabilirlik ve kanıt kalitesini değerlendirir.

**5. Kritik Akıl Yürütme Kontrol Listesi Super Prompt v1.0**  
Mantık hatalarını arar: yanlış nedensellik, acele genelleme, kategori hatası, anakronizm, kavram kayması vb.

**6. Tree of Thoughts Super Prompt v1.0**  
Tek cevap yerine birden fazla düşünme yolu üretir; sonra en güçlü yaklaşımı seçer.

**7. ReAct Reasoning Super Prompt v1.0**  
Araştırma, gözlem, kontrol ve revizyon döngüsü kurar. Özellikle web, dosya veya kaynak incelemeli işler için.

**8. Karşı Görüş ve Red Team Super Prompt v1.0**  
Bir cevaba saldırır; zayıf halkaları, karşı argümanları ve alternatif açıklamaları çıkarır.

**9. Kaynak Güvenilirliği Denetimi Super Prompt v1.0**  
Kaynakların türünü, güvenilirliğini, güncelliğini, çıkar çatışmasını ve iddiayı gerçekten destekleyip desteklemediğini inceler.

**10. Karar Matrisi ve Seçenek Değerlendirme Super Prompt v1.0**  
Birden fazla seçeneği kriter, ağırlık, puan, risk ve nihai öneriyle değerlendirir.

**11. Nihai Cevap Sadeleştirme ve Yönetici Özeti Super Prompt v1.0**  
Uzun analizi BLUF, ana bulgular, riskler, karar noktası ve aksiyon önerisine indirger.