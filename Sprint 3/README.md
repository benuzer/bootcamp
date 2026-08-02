# Sprint 3

**Sprint tarihleri:** 20 Temmuz 2026 – 2 Ağustos 2026
**Sprint hedefi:** Sprint 2'de çekirdeği kurulan ürünü, gerçekten çalışan ve uçtan uca kullanılabilen bir asistana dönüştürmek; kalan backlog story'lerini tamamlamak ve ürünü final teslime hazır hale getirmek.

---

## Sprint İçinde Tahmin Edilen Puan

- Product Backlog toplam puanı: **16 puan** (5 story)
- Sprint 1 sonunda tamamlanan: 0 puan (planlama sprinti)
- Sprint 2 sonunda tamamlanan: **8 puan** (Story 1, Story 5)
- Bu sprint hedefi: kalan **8 puan** (Story 2, Story 3, Story 4, Story 6) + backlog'a sprint içinde eklenen Story 7 (toplantı türüne göre özelleştirme, 3 puan)

## Backlog Dağıtma Mantığı

Sprint 2 sonunda Dify'a geçiş kararı çoktan alınmıştı ve çalışan bir özet üretme akışı kurulmuştu; ancak bu akış henüz bir arayüze bağlanmamıştı. Sprint 3'ün önceliği, kalan çekirdek story'leri (görev listesi, takip maili, sonraki toplantı gündemi) tek bir Dify prompt'unda birleştirip, Dify API'sine bağlı, çalışan bir HTML arayüz oluşturmaktı.

Geliştirme sürecinde kapsam genişledi (girdi türü önceliği, ses yükleme alanı, görevlerin kişi/taraf bazlı gruplanması, Gmail'e taslak olarak düşme, çoklu dil desteği, geçmiş kayıtlar); bu geliştirmeler Story 6 ve Story 7'yi de bu sprint içinde tamamlanır hale getirdi.

### Product Backlog

| # | Story | Puan | Durum |
|---|-------|------|-------|
| 1 | Transkript yapıştırıp özet alma *(çekirdek)* | 3 | Done (Sprint 2) |
| 5 | Ses dosyası yükleyip metne çevirme | 5 | Done (Sprint 2) |
| 2 | Görev listesi çıkarma *(çekirdek)* | 3 | **Done (Sprint 3)** |
| 3 | Müşteriye takip maili üretme *(çekirdek)* | 3 | **Done (Sprint 3)** |
| 4 | Sonraki toplantı gündemi üretme | 2 | **Done (Sprint 3)** |
| 6 | Geçmiş toplantıları görüntüleme | 3 | **Done (Sprint 3)** |
| 7 | Toplantı türüne göre özelleştirme *(iç toplantı / müşteri görüşmesi)* | 3 | **Done (Sprint 3)** |

**Product Backlog (Miro):** [Miro Board](https://miro.com/app/board/uXjVH-qS2yM=/?share_link_id=828504705814)

### Bu Sprinte Seçilen Story'ler

Sprint Planning'de To Do'ya alınan story'ler: **Story 2, 3, 4, 6 ve 7.**
Sprint sonunda backlog'daki tüm story'ler tamamlanmıştır.

## Daily Scrum

Daily Scrum toplantıları, ekip üyelerinin farklı saatlerde müsait olması nedeniyle yazılı olarak yürütülmüştür. Slack üzerinden iletişim sağlanamadığı için bu sprintte WhatsApp grubuna geçilmiştir.

**20 Temmuz 2026 — Sprint Planning**
- Sprint 2'nin değerlendirmesi yapıldı: Dify akışı çalışıyor ancak bir arayüze bağlı değil.
- Bu sprintin hedefi, kalan story'leri tamamlamak ve ürünü bir arayüze bağlamak olarak belirlendi.
- Bu sprinte aday story'ler To Do'ya alındı: Story 2, 3, 4, 6, 7.

**Sprint boyunca ürün geliştirme**
- İrem'in ürettiği ilk HTML dosyası üzerinden Melike geliştirmeleri yaptı, arayüzü otomasyona bağladı ve ürünü son haline getirdi.
- Ebuzer'in Sprint 1 ve 2'de geliştirmiş olduğu otomasyonda Melike son geliştirmeleri ve düzenlemeleri yaptı: görev listesi kişi bazlı (iç toplantı) ve taraf bazlı (müşteri görüşmesi) gruplandı (Story 2, Story 7); takip maili (Story 3) ve sonraki toplantı gündemi (Story 4) çıktıları, Dify promptlarının arayüzdeki dört bölümle birebir eşleşecek şekilde güncellenmesiyle tamamlandı.
- Arayüzde girdi türü önceliği (transkript / ses) netleştirildi, ses dosyası yükleme alanı eklendi, çoklu dil desteği (Türkçe/İngilizce) sağlandı.
- Takip mailinin doğrudan Gmail'de taslak olarak açılması sağlandı; geçmiş analizleri kaydedip tekrar görüntüleme özelliği eklendi (Story 6).
- Google Takvim'e ekleme özelliği değerlendirildi, kapsam dışı bırakılmasına karar verildi.
- Ürünün demo videosu çekildi ve final teslime hazırlandı.

Daily Scrum konuşmalarının ekran görüntüleri:

<img src="./images/Screenshot%202026-08-02%20at%2015.09.57.png" width="420" alt="Daily Scrum 1"><br>
<img src="./images/Screenshot%202026-08-02%20at%2015.10.20.png" width="420" alt="Daily Scrum 2"><br>
<img src="./images/Screenshot%202026-08-02%20at%2015.10.42.png" width="420" alt="Daily Scrum 3"><br>
<img src="./images/Screenshot%202026-08-02%20at%2015.12.09.png" width="420" alt="Daily Scrum 4"><br>
<img src="./images/Screenshot%202026-08-02%20at%2019.14.42.png" width="420" alt="Daily Scrum 5">

## Sprint Board Update

Sprint board ekran görüntüsü (Product Backlog + To Do / In Progress / Done):

<img src="./images/sprint-board-3.png" width="600" alt="Sprint Board">

## Ürün Durumu

Bu sprint sonunda ürün, çalışan bir web arayüzüne dönüştürülmüştür. Kullanıcı transkript yapıştırabilir ya da ses dosyası yükleyebilir; toplantı türü, çıktı dili ve mail tonu seçebilir. Ürün, Dify üzerinden çalışan yapay zeka akışıyla toplantı özetini, sorumlusuna göre gruplanmış görev listesini, doğrudan Gmail'e taşınabilir takip mailini ve bir sonraki toplantı gündemini üretir. Ayrıca geçmiş analizler kaydedilip tekrar görüntülenebilir.

<img src="./images/urun-durumu-3.png" width="600" alt="Ürün Durumu">

Ürünün çalışan halinin kısa demosu:

[Demo Videosu](./images/OTOPILOT-DEMO.mp4)

## Sprint Review

Bu sprint, ürünün planlama ve tasarım aşamasından uçtan uca çalışan bir asistana dönüştüğü geliştirme sprintidir. Sprint boyunca yapılanlar:

- İrem'in ürettiği ilk HTML dosyası üzerinden Melike geliştirmeleri yaptı ve Dify API'sine bağlı, çalışan bir arayüze (otopilot-app.html) dönüştürdü.
- Görev listesi, takip maili ve sonraki toplantı gündemi üretimi tek bir prompt yapısında birleştirildi.
- Geliştirme sürecinde arayüz iyileştirildi: ses yükleme alanı, gruplu görev listesi, Gmail entegrasyonu, çoklu dil desteği, geçmiş kayıtlar.
- Product Backlog'daki tüm story'ler (2, 3, 4, 6, 7) tamamlandı.
- Ürünün demo videosu çekildi ve final teslime hazırlandı.

**Tamamlanan:** Story 2, 3, 4, 6, 7 — backlog'un tamamı.
**Sonraki sprinte taşınan:** Yok — bu, projenin son sprintidir.
**Katılımcılar:** İpek Ilgın Şimşek, Melike Yıldız, Ebuzer Yitiz, İrem Tosun.

## Sprint Retrospective

**İyi giden:**
- [Ekip birer cümle ekleyecek — ör. "Dify'a geçiş, akışı ön yüze bağlamayı çok kolaylaştırdı."]

**Geliştirilebilecek:**
- Ekip içi katılımın sprint boyunca daha dengeli olması; bazı üyelerin ilerlemesini paylaşma sıklığı artırılabilir.
- [Ekip ekleyecek]

**Sonraki adımlar için notlar:**
- Ürün fikri devam ettirilecek olursa, ek entegrasyonlarla (ör. CRM) genişletilebilir.
- [Ekip ekleyecek]
