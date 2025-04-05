# Ekonomi Yönetimi Uygulaması

Bu uygulama, kişisel harcamaları, abonelikleri ve finansal durumu takip etmek için geliştirilmiş bir mobil uygulamadır.

## Özellikler

- Harcama ve gelir takibi
- Abonelik yönetimi ve hatırlatıcıları
- Finans analizi ve istatistikler
- Ödeme bildirimleri
- Modern ve kullanıcı dostu arayüz

## Google Play Store'a Yükleme Adımları

### 1. Gerekli Ayarları Yapma

`app.json` dosyasında aşağıdaki bilgileri kendi uygulama bilgilerinize göre düzenleyin:

- `name`: Uygulama adı
- `package`: Android paket adı (örn. com.sirketiniz.uygulamaadi)
- `versionCode`: Sürüm kodu (her yeni sürümde artırılmalı)
- `versionName`: Sürüm adı (kullanıcıların göreceği versiyon)

### 2. İkonları ve Splash Screen'i Düzenleme

Uygulamanız için profesyonel ikonlar oluşturun ve aşağıdaki dosyaları güncelleyin:

- `./assets/icon.png`: 1024x1024 px ana ikon
- `./assets/adaptive-icon.png`: 1024x1024 px Android uyarlanabilir ikon
- `./assets/notification-icon.png`: 96x96 px bildirim ikonu
- `./assets/splash.png`: 1242x2436 px açılış ekranı

### 3. Build Alma

AAB (Android App Bundle) oluşturmak için:

```bash
eas build --platform android --profile production
```

APK (test için) oluşturmak için:

```bash
eas build --platform android --profile preview
```

### 4. Google Play Console'a Yükleme

1. [Google Play Console](https://play.google.com/console/)'a gidin
2. Yeni uygulama oluşturun veya var olan uygulamayı seçin
3. "Üretim" bölümünden yeni bir sürüm oluşturun
4. AAB dosyasını yükleyin
5. Uygulama bilgilerini, ekran görüntülerini ve açıklamaları ekleyin
6. Gerekli form ve beyanları doldurun
7. İnceleme için gönderin

### 5. Google Play Console Gerekli Materyaller

- Kısa açıklama (80 karakter)
- Tam açıklama (4000 karakter)
- En az 8 ekran görüntüsü (farklı cihaz türleri için)
- Özellik grafiği (1024x500 px)
- Uygulama ikonu (512x512 px)
- Gizlilik politikası linki

## Kullanılan Teknolojiler

- React Native
- Expo
- React Native Paper
- Async Storage
- Expo Notifications

## Sorular ve Destek

Uygulama ile ilgili sorularınız veya teknik destek için iletişime geçin.

### Not

Bu dokümantasyon, uygulamanın Google Play Store'a yüklenmesi için temel adımları içerir. Google Play politikaları ve gereksinimleri zamanla değişebilir, güncel bilgiler için [Google Play Console Yardım](https://support.google.com/googleplay/android-developer) sayfasını kontrol edin. 