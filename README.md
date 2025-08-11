# STM32 DS3231 RTC I²C Örneği

<img width="1187" height="736" alt="aa" src="https://github.com/user-attachments/assets/5d260f0e-2bc1-45ee-9253-c8a95ba74f81" />


Bu proje, STM32 mikrodenetleyici kullanarak **DS3231 Gerçek Zaman Saati (RTC)** modülünden I²C protokolü ile tarih ve saat okuma/yazma işlemlerini gösteren bir örnek uygulamadır.

## 📌 Özellikler
- DS3231 RTC ile I²C üzerinden haberleşme
- Saat, dakika, saniye, gün, ay, yıl verilerini ayarlama
- DS3231'den düzenli aralıklarla veri okuma
- HAL kütüphanesi ile kolay I²C kullanımı

## 📂 Proje Yapısı
- **main.c** → RTC ayarlama ve okuma fonksiyonları, I²C yapılandırması
- **DS3231_Time_t** → Tarih-saat verilerini tutan yapı
- **DEC_To_BCD / BCD_To_DEC** → Sayı format dönüşüm fonksiyonları

## 🔌 Donanım Bağlantıları
| STM32 Pin | DS3231 Pin |
|-----------|-----------|
| PB6 (SCL) | SCL       |
| PB7 (SDA) | SDA       |
| GND       | GND       |
| 3.3V / 5V | VCC       |

## 🛠️ Geliştirme Ortamı
- **MCU**: STM32 (CubeMX ile yapılandırılmış)
- **IDE**: STM32CubeIDE
- **Bağlantı**: I²C (400 kHz)

## 📜 Lisans
Bu proje, STM32CubeIDE tarafından oluşturulan temel HAL yapısını kullanır ve STM32CubeMX lisans koşullarına tabidir.
