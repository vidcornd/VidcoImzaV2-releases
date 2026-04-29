# VidcoImzaV2-releases

============================================================
  Vidco e-İmza v2.0.0 — Windows Kurulum Kılavuzu
============================================================

Desteklenen Windows sürümleri:
  - Windows 10 (1809 ve üzeri)
  - Windows 11
  - Windows Server 2016, 2019, 2022

NOT: Windows 7, 8 ve 8.1 desteklenmemektedir.


------------------------------------------------------------
ADIM 1: OpenSC Kurulumu (Akıllı Kart Sürücüsü)
------------------------------------------------------------
Akıllı kartınızı (e-imza tokenını) okumak için OpenSC gereklidir. 
(Eğer e-imza sağlayıcınızın sürücüsünü kurduysanız bu adımı atlayın)

1. Aşağıdaki adresi tarayıcınızda açın:
   https://github.com/OpenSC/OpenSC/releases/latest

2. "OpenSC-X.Y.Z_win64.msi" dosyasını indirin.

3. İndirilen .msi dosyasını çalıştırın ve kurulumu tamamlayın.

NOT: Bazı kurumsal kartlar (EİMZATR, TÜBİTAK, TürkTrust, E-Güven)
     OpenSC ile sorunsuz çalışmaktadır.


------------------------------------------------------------
ADIM 2: Vidco e-İmza Kurulumu
------------------------------------------------------------
Java kurulumuna gerek yoktur — uygulama her şeyi içinde barındırır.

1. "VidcoImza-2.0.0.exe" dosyasını çalıştırın.

2. Kurulum sihirbazını takip edin ve tamamlayın.

3. Masaüstünde veya Başlat menüsünde oluşturulan
   "VidcoImza" kısayoluna çift tıklayarak uygulamayı açın.


------------------------------------------------------------
ADIM 3: Kullanım
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
  Vidco e-İmza v2.0.0 — MACOS Kurulum Kılavuzu
============================================================
1. Java Kurulumu Yapın

2. E-imza sürücüsünü Kurun
   
3. VidcoImza.command dosyasını çift tıklayın

4. Kullanım adımları ile devam edin

------------------------------------------------------------
GÜNCELLEME
------------------------------------------------------------
Yeni bir sürüm mevcut olduğunda uygulama açılışında otomatik
olarak bildirim gösterir. "Güncelle" seçeneğine tıklamanız
yeterlidir — güncelleme otomatik uygulanır.


------------------------------------------------------------
SIKÇA KARŞILAŞILAN SORUNLAR
------------------------------------------------------------

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


------------------------------------------------------------
İletişim
------------------------------------------------------------
Sorun yaşamanız durumunda lütfen aşağıdaki bilgilerle
BT destek ekibinize ulaşın:

  - Hata mesajının tam metni
  - Log dosyasının konumu:
    C:\Users\<KullanıcıAdı>\VidcoImzaV2\debug\vidcoimza.log

============================================================

