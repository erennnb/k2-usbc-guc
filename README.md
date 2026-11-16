# K2 — USB-C Güç Kartı

USB-C'den aldığı 5 V'u 3.3 V'a düşüren küçük bir güç kartı.

## Gereksinimler
- **Giriş:** USB-C, yalnız güç, 5 V
- **Çıkış:** 3.3 V, en az 500 mA
- **Koruma:** polyfuse (aşırı akım) + TVS (gerilim darbesi)
- **Ekstralar:** güç LED'i, çıkış header'ı (5V, 3V3, GND), test noktaları
- **Kart:** 2 katman, en fazla 40×30 mm

## Parça seçimleri
| Parça | LCSC no | JLCPCB | Not |
|---|---|---|---|
| USB-C konnektör (6 pin) | C456012 | Extended | SHOU HAN TYPE-C 6P, SMD, R/A |

## CC dirençleri (5.1 kΩ)
CC1 ve CC2 pinlerinin her biri ayrı bir 5.1 kΩ dirençle GND'ye bağlanır.

<!-- Buraya 2–3 cümleyle kendin yaz:
     1) Bu dirençler ne işe yarıyor?
     2) İkisini neden tek dirençle birleştiremeyiz?
     3) Hiç direnç koymazsan ne olur? -->