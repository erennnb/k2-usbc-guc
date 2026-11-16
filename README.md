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
| CC dirençleri (×2) | C27834 | Basic | 5.1 kΩ, %1, 0805 |
| Polyfuse | C5144563 | Extended | FSMD075-1206R · 1206, I_hold 0.75 A, V_max 8 V |
| TVS | C83329 | Extended | SMAJ6.0A · tek yönlü, V_R 6.0 V, V_C 10.3 V |
| C_in | C15850 | Basic | 10 µF, 25 V, X5R, 0805 (Samsung CL21A106KAYNNNE) |
| 3.3 V LDO | C6186 | Basic | AMS1117-3.3, SOT-223 · 500 mA'de ~0.85 W kayıp → tab altına bakır alan |
| C_out | C7198 | Extended | 22 µF, 10 V tantal, B kılıf (3528), ESR 2.4 Ω |
| Güç LED'i | C84256 | Basic | Kırmızı, 0805, V_F 1.6–2.6 V |
| LED direnci | C17513 | Basic | 1 kΩ, %1, 0805 → I_LED ≈ 1.3 mA |
| Çıkış header'ı | — | — | 1×3, 2.54 mm, THT (5V, 3V3, GND) |
| Test noktaları | — | — | PCB pad'i (5V, 3V3, GND) |





## CC dirençleri (5.1 kΩ)
CC1 ve CC2 pinlerinin her biri ayrı bir 5.1 kΩ dirençle GND'ye bağlanır.

<!-- Buraya 2–3 cümleyle kendin yaz:
     1) Bu dirençler ne işe yarıyor? anlamadım,
     2) İkisini neden tek dirençle birleştiremeyiz?anlamadım
     3) Hiç direnç koymazsan ne olur? -->