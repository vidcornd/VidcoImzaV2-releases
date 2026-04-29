============================================================
  Vidco e-İmza v2.0.0 — Kurulum Kılavuzu
============================================================

Desteklenen platformlar:
  - Windows 10 (1809 ve üzeri), Windows 11
  - Windows Server 2016, 2019, 2022
  - macOS 12 Monterey ve üzeri (Intel ve Apple Silicon)

NOT: Windows 7, 8 ve 8.1 desteklenmemektedir.


============================================================
  WINDOWS
============================================================

------------------------------------------------------------
ADIM 1: Akıllı Kart Sürücüsü Kurulumu
------------------------------------------------------------
Uygulama aşağıdaki sürücüleri otomatik olarak tanır.
Bunlardan yalnızca birini kurmanız yeterlidir:

  • Kart sağlayıcınızın kendi yazılımı (önerilen):
      - EİMZATR  → https://www.eimzatr.com/destek
      - TürkTrust → https://www.turktrust.com.tr
      - TÜBİTAK Akis → https://kamusm.bilgem.tubitak.gov.tr
      - E-Güven  → https://www.e-guven.com
      - E-Tuğra  → https://www.e-tugra.com.tr
      - ArkSigner → https://www.arksigner.com

  • Veya OpenSC (evrensel sürücü):
      https://github.com/OpenSC/OpenSC/releases/latest
      → "OpenSC-X.Y.Z_win64.msi" dosyasını indirip kurun.

Sağlayıcınızın yazılımı zaten kuruluysa bu adımı atlayabilirsiniz.


------------------------------------------------------------
ADIM 2: Vidco e-İmza Kurulumu
------------------------------------------------------------
Java kurulumuna gerek yoktur — uygulama her şeyi içinde barındırır.

1. "VidcoImza-2.0.0.exe" dosyasını çalıştırın.

2. Kurulum sihirbazını takip edin ve tamamlayın.

3. Masaüstünde veya Başlat menüsünde oluşturulan
   "VidcoImza" kısayoluna çift tıklayarak uygulamayı açın.


------------------------------------------------------------
ADIM 3: Kullanım (Windows)
------------------------------------------------------------
1. Kart okuyucunuzu bilgisayara takın.

2. E-imza kartınızı kart okuyucuya yerleştirin.

3. Uygulamayı açın:
   a) "Cihazları Tara" butonuna tıklayın.
   b) Açılan listeden kartınızın bulunduğu okuyucuyu seçin.
   c) PIN kodunuzu girin.
   d) Domain alanına sunucu adresinizi yazın.
   e) "İMZALA" butonuna tıklayın.


============================================================
  MACOS
============================================================

------------------------------------------------------------
ADIM 1: Akıllı Kart Sürücüsü Kurulumu
------------------------------------------------------------
Uygulama aşağıdaki sürücüleri otomatik olarak tanır.
Bunlardan yalnızca birini kurmanız yeterlidir:

  • Kart sağlayıcınızın kendi yazılımı (önerilen):
      - EİMZATR  → https://www.eimzatr.com/destek
      - TürkTrust → https://www.turktrust.com.tr
      - TÜBİTAK Akis → https://kamusm.bilgem.tubitak.gov.tr
      - E-Güven  → https://www.e-guven.com
      - E-Tuğra  → https://www.e-tugra.com.tr
      - ArkSigner → https://www.arksigner.com

  • Veya OpenSC (evrensel sürücü):
      https://github.com/OpenSC/OpenSC/releases/latest
      → "OpenSC-X.Y.Z.dmg" dosyasını indirip kurun.

Sağlayıcınızın yazılımı zaten kuruluysa bu adımı atlayabilirsiniz.


------------------------------------------------------------
ADIM 2: Java Kurulumu
------------------------------------------------------------
macOS sürümü için Temurin Java 21 (x64) gereklidir.

1. Aşağıdaki adresi tarayıcınızda açın:
   https://adoptium.net/temurin/releases/?version=21&os=mac&arch=x64

2. "macOS x64" satırındaki ".pkg" dosyasını indirin.

3. İndirilen .pkg dosyasını çalıştırın ve kurulumu tamamlayın.

NOT: Apple Silicon (M1/M2/M3) kullanıyorsanız yine de
     x64 sürümünü indirin — uygulama Rosetta ile çalışır.


------------------------------------------------------------
ADIM 3: Vidco e-İmza Kurulumu
------------------------------------------------------------
1. "VidcoImza-mac-2.0.0.zip" dosyasını indirin.

2. Zip dosyasını açın — iki dosya çıkacak:
     vidcoimza-mac.jar
     VidcoImza.command

3. Her iki dosyayı aynı klasörde bırakın.
   (Örneğin: Uygulamalar veya masaüstü klasörünüz)

4. "VidcoImza.command" dosyasına çift tıklayın.
   İlk açılışta "Geliştirici Doğrulanamıyor" uyarısı çıkarsa:
   → Sistem Ayarları > Gizlilik ve Güvenlik > "Yine de Aç"


------------------------------------------------------------
ADIM 4: Kullanım (macOS)
------------------------------------------------------------
1. Kart okuyucunuzu bilgisayara takın.

2. E-imza kartınızı kart okuyucuya yerleştirin.

3. Uygulamayı açın:
   a) "Cihazları Tara" butonuna tıklayın.
   b) Açılan listeden kartınızın bulunduğu okuyucuyu seçin.
   c) PIN kodunuzu girin.
   d) Domain alanına sunucu adresinizi yazın.
   e) "İMZALA" butonuna tıklayın.


============================================================
  GÜNCELLEME
============================================================
Yeni bir sürüm mevcut olduğunda uygulama açılışında otomatik
olarak bildirim gösterir. "Güncelle" seçeneğine tıklamanız
yeterlidir — güncelleme otomatik uygulanır.

Windows ve macOS için güncelleme ayrı ayrı çalışır,
ek bir işlem yapmanıza gerek yoktur.


============================================================
  SIKÇA KARŞILAŞILAN SORUNLAR
============================================================

SORUN : Kart okuyucu listede görünmüyor
ÇÖZÜM : OpenSC'nin kurulu olduğundan emin olun (Adım 1).
         Okuyucuyu farklı bir USB portuna takın.
         "Cihazları Tara" butonuna tekrar basın.

SORUN : PIN hatalı uyarısı
ÇÖZÜM : PIN'i dikkatlice girin. Çoğu kart 3 yanlış denemede
         kilitlenir. Emin değilseniz kartı çıkarıp tekrar takın.

SORUN : Sunucuya bağlanılamadı
ÇÖZÜM : İnternet bağlantınızı ve Domain alanındaki adresi
         kontrol edin. Güvenlik duvarı veya proxy engelliyor
         olabilir — BT departmanınıza danışın.

SORUN : Sertifika doğrulanamıyor
ÇÖZÜM : Kartın TÜBİTAK, TürkTrust, EİMZATR, E-Güven veya
         E-Tuğra onaylı Nitelikli Elektronik Sertifika (NES)
         içerdiğinden emin olun. OpenSC'yi kaldırıp yeniden
         kurun.

SORUN : macOS — "Geliştirici Doğrulanamıyor" hatası
ÇÖZÜM : Sistem Ayarları > Gizlilik ve Güvenlik bölümünde
         "Yine de Aç" seçeneğine tıklayın.

SORUN : macOS — Uygulama açılmıyor (Java bulunamadı)
ÇÖZÜM : Adım 2'deki Java kurulumunu tamamladığınızdan ve
         x64 sürümünü indirdiğinizden emin olun.


============================================================
  İletişim
============================================================
Sorun yaşamanız durumunda lütfen aşağıdaki bilgilerle
BT destek ekibinize ulaşın:

  - Hata mesajının tam metni
  - Log dosyasının konumu:

    Windows:
    C:\Users\<KullanıcıAdı>\VidcoImzaV2\debug\vidcoimza.log

    macOS:
    /Users/<KullanıcıAdı>/VidcoImzaV2/debug/vidcoimza.log

============================================================
