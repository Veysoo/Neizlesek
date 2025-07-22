# 🎬 Neizlesek – Yapay Zekâ Destekli Film ve Dizi Öneri Platformu

**Neizlesek**, kullanıcıların izledikleri, beğendikleri ve izlemek istedikleri film ve dizileri takip edebilecekleri, ayrıca yapay zekâ destekli kişiselleştirilmiş öneriler alabilecekleri modern bir web uygulamasıdır.

## 🚀 Özellikler

- 🔍 Kişiselleştirilmiş film/dizi öneri sistemi (AI destekli)
- 🎞 İzlenen, beğenilen, izlenmek istenen içerik listeleri
- 🌟 Yeni çıkanlar, trend olanlar, popüler içerikler
- 🧠 Firebase Authentication ile güvenli kullanıcı girişi
- ☁️ Firebase Firestore ile veri saklama
- 🖼 Modern ve responsive arayüz (React + CSS/SCSS)
- 💡 İçerik açıklamaları, fragmanlar, IMDB gibi metriklerle detay sayfası

---

## 🏗️ Kullanılan Teknolojiler

| Teknoloji          | Açıklama                                  |
| ------------------ | ----------------------------------------- |
| React              | Kullanıcı arayüzü                         |
| Firebase           | Authentication, Firestore, Storage        |
| SCSS / CSS Modules | Modern ve modüler stilleme                |
| TMDB API           | Film/Dizi bilgileri için (isteğe bağlı)   |
| OpenAI API         | İçerik öneri ve analizleri (isteğe bağlı) |

---

## 📁 Proje Yapısı (Sayfalar)

src/
│
├── pages/
│ ├── Home.tsx // Ana sayfa: yeni çıkanlar, trend içerikler
│ ├── Profile.tsx // Kullanıcıya özel profil
│ ├── Watchlist.tsx // İzlemek istenenler
│ ├── Watched.tsx // İzlenenler
│ ├── Favorites.tsx // Beğenilenler
│ ├── Recommendations.tsx // AI destekli öneriler
│ └── Details.tsx // İçerik detay sayfası
│
├── components/
│ ├── Navbar.tsx
│ ├── ContentCard.tsx
│ ├── SearchBar.tsx
│ ├── LoginModal.tsx
│ └── RecommendationCard.tsx
│
└── firebase/
└── firebaseConfig.ts

---

## 🎨 Arayüz Tasarım Önerisi

🔹 **Navbar (üst menü)**

- Logo, arama çubuğu, kullanıcı simgesi
- Koyu tema desteği, sezgisel geçiş animasyonları

🔹 **Content Cards (film/dizi kutuları)**

- Poster, başlık, tür, butonlar: ⭐ Ekle | 👀 İzlendi | ➕ Watchlist
- Hover efektiyle öne çıkan bilgiler (rating, yıl vs.)

🔹 **Detay Sayfası**

- Arka planda blur poster
- Frag

---

## 🎨 Arayüz Tasarım Önerisi

🔹 **Navbar (üst menü)**

- Logo, arama çubuğu, kullanıcı simgesi
- Koyu tema desteği, sezgisel geçiş animasyonları

🔹 **Content Cards (film/dizi kutuları)**

- Poster, başlık, tür, butonlar: ⭐ Ekle | 👀 İzlendi | ➕ Watchlist
- Hover efektiyle öne çıkan bilgiler (rating, yıl vs.)

🔹 **Detay Sayfası**

- Arka planda blur poster
- Fragman (YouTube iframe)
- AI destekli açıklama/öneri kutusu (örn. "Bunu sevdiysen, şunlara da göz at")

🔹 **Profil Sayfası**

- Kullanıcının etkinlik geçmişi, listeleri ve tercih ayarları
- UI: Kart grid yapısı, responsive, sade & estetik

---

🧠 Yapay Zekâ / Öneri Sistemi (Opsiyonel)
Kullanıcının beğendiği türler, izlediği içerikler analiz edilerek benzer içerikler önerilir.

Basit örnek için içeriklere kategori tag’leri ekleyip benzerlerini filtreleyebilirsiniz.

Gelişmiş versiyon: OpenAI API ile açıklamaya dayalı içerik benzerliği çıkarımı yapılabilir.

✨ Geliştirme Notları
Mobil uyum önemlidir: sayfalar responsive olmalı.

Erişilebilirlik (a11y) kontrollerine dikkat edin.

Lazy loading ile performans artırılabilir.

Kullanıcı tercihlerine göre öneri sistemi güncellenebilir.

📌 Yol Haritası
AI destekli öneri sisteminin entegrasyonu

Kullanıcı takip sistemi (arkadaşlar ne izliyor?)

Bildirimler / izleme hatırlatıcıları

Dark / Light tema geçişi
