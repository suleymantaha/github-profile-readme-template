# 📋 Detaylı Kurulum Kılavuzu

## Adım 1: Repo Oluşturma

1. Bu repoyu **Use this template** ile kopyalayın
2. Yeni repo adı: **`kullaniciadiniz`** (GitHub kullanıcı adınızla aynı)
3. Public olarak oluşturun

> ⚠️ GitHub profil README'si için repo adı **kullanıcı adıyla aynı** olmalıdır (örn: `johndoe/johndoe`)

## Adım 2: Dosya Hazırlığı

```bash
# TEMPLATE_README.md içeriğini README.md'ye kopyalayın
cp TEMPLATE_README.md README.md
```

## Adım 3: Değiştirilecek Placeholder'lar

### README.md içinde:

| Placeholder | Değiştir | Örnek |
|-------------|----------|-------|
| `YOUR_USERNAME` | GitHub kullanıcı adınız | `johndoe` |
| `YOUR_EMAIL` | E-posta adresiniz | `john@example.com` |
| `YOUR_LINKEDIN` | LinkedIn kullanıcı adı | `johndoe` |
| `YOUR_REPO_1` | 1. öne çıkan proje | `awesome-project` |
| `YOUR_REPO_2` | 2. öne çıkan proje | `another-project` |

### Typing animasyonu

`lines=` parametresindeki metinleri değiştirin. Satırlar `+` ile birleştirilir, `;` ile ayrılır:

```
lines=First+line;Second+line;Third+line
```

### .github/workflows/update-stats.yml içinde:

| Placeholder | Değiştir |
|-------------|----------|
| `YOUR_REPO_1` | İlk öne çıkan proje repo adı |
| `YOUR_REPO_2` | İkinci öne çıkan proje repo adı |

> Workflow'da `username` otomatik alınır (`${{ github.repository_owner }}`) — profil repo formatında repo sahibi = kullanıcı adınız.

## Adım 4: İlk Push ve Workflow

1. Değişiklikleri commit edip push edin
2. **Actions** → **Update Profile Stats** → **Run workflow**
3. 2-3 dakika bekleyin
4. `profile/` klasörü SVG dosyalarıyla dolacak

## Adım 5: Katkı Yılanı (Opsiyonel)

[Platane/snk](https://github.com/Platane/snk) kullanarak katkı yılanı ekleyin. Repo README'sindeki talimatları takip edin.

## Sorun Giderme

**SVG'ler görünmüyor?**  
→ Actions'da workflow'un başarıyla tamamlandığından emin olun. Hata varsa logları kontrol edin.

**Pin kartları boş?**  
→ `YOUR_REPO_1` ve `YOUR_REPO_2`'nin var olan public repolarınız olduğundan emin olun.

**Trophy yüklenmiyor?**  
→ `gh-trophy.cdnsoft.net` alternatif servis kullanılıyor. Sorun devam ederse [ryo-ma/github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy) load balancing URL'lerini deneyin.
