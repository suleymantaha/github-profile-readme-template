# 🎨 GitHub Profile README Template

GitHub profil README'nizi etkileyici hale getirmek için hazır şablon. **Rate limit** ve **yükleme sorunlarına** karşı istatistikler **yerel SVG** olarak saklanır, GitHub Actions ile otomatik güncellenir.

## 📸 Önizleme

Profil README şablonunun nasıl görüneceğini görmek için:

**[→ Şablon önizlemesini görüntüle](https://github.com/suleymantaha/github-profile-readme-template/blob/main/TEMPLATE_README.md)**

*(Tıklayın — GitHub'da render edilmiş hali açılır)*

---

## ✨ Özellikler

- 📊 GitHub Stats, Top Languages, Streak
- 🏆 Başarı rozetleri (Trophy)
- 📈 31 günlük katkı grafiği
- 📌 Öne çıkan proje kartları (2 adet)
- 🛠️ Teknoloji stack ikonları
- 🐍 Katkı yılanı (ayrı kurulum gerekir)
- ⏰ Her 6 saatte otomatik güncelleme

## 🚀 Hızlı Kurulum

### 1. Template'i Kullan

Bu repoyu **Use this template** ile kopyalayın. Yeni repo adı **kullanıcı adınızla aynı** olmalı (örn: `johndoe/johndoe`) — bu GitHub profil README formatıdır.

### 2. Dosyaları Kopyala

- `TEMPLATE_README.md` → `README.md` olarak yeniden adlandırın
- `.github/workflows/` klasörü zaten dahil

### 3. Kişiselleştir

| Değiştir | Dosya | Açıklama |
|----------|-------|----------|
| `YOUR_USERNAME` | README.md, workflow | GitHub kullanıcı adınız |
| `YOUR_REPO_1`, `YOUR_REPO_2` | `.github/workflows/update-stats.yml` | Öne çıkarmak istediğiniz 2 repo |
| Typing satırları | README.md | `lines=` parametresindeki metinler |
| E-posta, LinkedIn | README.md | İletişim bilgileriniz |
| Renkler | workflow, README | `title_color`, `icon_color` vb. |

### 4. İlk Çalıştırma

Push sonrası **Actions** sekmesinden workflow'u manuel tetikleyin veya 6 saat bekleyin. `profile/` klasörü oluşacak.

## 📁 Klasör Yapısı

```
.
├── README.md              ← Profil README (TEMPLATE_README.md'dan)
├── .github/
│   └── workflows/
│       └── update-stats.yml
└── profile/               ← SVG'ler buraya (otomatik)
    ├── stats.svg
    ├── top-langs.svg
    ├── streak.svg
    ├── trophy.svg
    ├── activity.svg
    └── pin-*.svg
```

## 🐍 Katkı Yılanı (Opsiyonel)

[Platane/snc](https://github.com/Platane/snk) ile katkı yılanı eklemek için ayrı workflow gerekir. [Bu örnek](https://github.com/Platane/snk#github-action) ile kurabilirsiniz.

## 🎨 Renk Özelleştirme

Workflow ve README'deki renk kodlarını değiştirin:

- `title_color` — Başlık rengi
- `icon_color` — İkon rengi  
- `text_color` — Metin rengi

## 📄 Lisans

MIT — İstediğiniz gibi kullanın.

---

**Not:** Bu template herhangi bir kişiye veya organizasyona özel değildir. Kendi GitHub kullanıcı adınız ve repolarınızla kişiselleştirmeniz yeterlidir.
