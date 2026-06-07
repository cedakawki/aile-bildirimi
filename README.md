[README.md](https://github.com/user-attachments/files/28685174/README.md)
# 📱 Aile Bildirimi Uygulaması

Anne'den tek tıkla aile bildirimi. GitHub Pages üzerinde ücretsiz çalışır, telefona uygulama gibi eklenebilir.

---

## 🚀 Adım 1 — Dosyaları GitHub'a yükle

1. [github.com](https://github.com) adresinde hesap aç (yoksa ücretsiz)
2. **New repository** → İsim: `aile-bildirimi` → **Public** → **Create**
3. Repository sayfasında **uploading an existing file** linkine tıkla
4. Şu dosyaları sürükle-bırak:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icons/` klasörü (192.png ve 512.png)
   - `.github/workflows/deploy.yml`
5. **Commit changes** butonuna bas

---

## 🌐 Adım 2 — GitHub Pages'i aç

1. Repository → **Settings** → Sol menüde **Pages**
2. **Source:** `GitHub Actions` seç
3. Birkaç dakika bekle → yeşil ✅ çıkınca site hazır
4. Adres: `https://KULLANICI_ADIN.github.io/aile-bildirimi`

---

## 🔔 Adım 3 — OneSignal kurulumu (farklı telefonlara bildirim)

> OneSignal olmadan sadece aynı sayfadaki bildirimler çalışır.
> Farklı telefona bildirim göndermek için OneSignal gerekli — **ücretsiz**.

1. [onesignal.com](https://onesignal.com) → ücretsiz hesap aç
2. **New App** → İsim: `Aile Bildirimi`
3. Platform: **Web** seç
4. Site URL: `https://KULLANICI_ADIN.github.io/aile-bildirimi`
5. **App ID** kopyala (uzun bir kod)
6. `index.html` dosyasını aç, şu satırı bul:
   ```
   appId: "ONESIGNAL_APP_ID_BURAYA",
   ```
   Oraya kopyaladığın App ID'yi yapıştır.
7. Dosyayı GitHub'a tekrar yükle → otomatik deploy olur

---

## 📲 Adım 4 — Telefona uygulama gibi ekle

### iPhone (Safari)
1. Safari'de `https://KULLANICI_ADIN.github.io/aile-bildirimi` aç
2. Alt çubuktaki **Paylaş** butonuna bas (kutu + ok ikonu)
3. **Ana Ekrana Ekle** seç
4. İsim: **Aile** → **Ekle**
5. Ana ekranda uygulama ikonu çıkar ✅

### Android (Chrome)
1. Chrome'da siteyi aç
2. Sağ üstteki **⋮ menü** → **Ana ekrana ekle** (veya otomatik banner çıkar)
3. **Ekle** → Ana ekranda ikon belirir ✅

---

## 👩 Anne için kullanım

- Telefona ikondan girer
- Büyük butonlardan birine basar (Yemek hazır, Çay hazır vb.)
- Aile telefonlarına bildirim gider ✅

---

## 👨‍👩‍👧 Aile üyeleri için

- Aynı linki telefonlarında açar
- Alt menüden **Aile** sekmesine geçer
- **Bildirimlere abone ol** butonuna basar → izin verir
- Artık anne mesaj gönderdiğinde bildirim alırlar ✅

---

## 🛠️ İleride eklenebilecekler

- Özel mesaj yazma
- Sesli uyarı seçimi
- Mesaj geçmişi
- Okundu bildirimi
- Dil seçeneği

---

Sorun yaşarsan README'yi bir AI'a göster, yardımcı olabilir 😊
