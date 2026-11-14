# Cari Takip Mobil (Android & iOS — Native Flutter)

Bu proje WebView kullanmayan, doğrudan Android ve iOS için derlenen **native Flutter** mobil uygulamasıdır ve PHP sunucunuzdaki `/api/` uç noktalarıyla JWT (Bearer Token) üzerinden haberleşir.

## Kurulum ve Derleme

1. `lib/services/api_service.dart` dosyasındaki `baseUrl` adresini kendi PHP sunucunuzun `/api` yoluna göre güncelleyin (ör. `https://alanadiniz.com/cari_takip/api`).
2. `cari_takip_sistemi/api/bootstrap.php` içindeki `JWT_SECRET_KEY` değerini güçlü bir anahtarla değiştirin.
3. Proje klasöründe paketleri yükleyin:
   ```bash
   flutter pub get
   ```
4. Android APK veya App Bundle üretin:
   ```bash
   flutter build apk --release
   ```
5. iOS (macOS üzerinde Xcode ile) derleyin:
   ```bash
   flutter build ios --release
   ```
