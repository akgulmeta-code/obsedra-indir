# OBSEDRA — indirme

Rolleri olan AI ajanlarından kurulmuş bir ofis. Görev yazarsın, iş doğru ajana gider, kanıtla kapanır.

Bu depo yalnız **kurulum dosyalarını** taşır; kaynak kod burada değildir.

**İndir:** [Sürümler](../../releases/latest) — Apple Silicon (M1–M4) ve Intel Mac için `.dmg`.

## Kurulum
1. İnen `.dmg` dosyasını aç, OBSEDRA'yı Uygulamalar klasörüne sürükle.
2. İlk açılışta **"OBSEDRA Açılmadı"** kutusu çıkar (uygulama henüz Apple tarafından imzalanmadı). **Bitti**'ye bas; *Çöp Sepeti'ne Taşı*'ya basma.
3. **Sistem Ayarları → Gizlilik ve Güvenlik**'in en altında "OBSEDRA engellendi" satırındaki **Yine de Aç**'a bas, Mac şifreni gir, tekrar **Aç** de. Bir kez yapılır.

"Yine de Aç" görünmüyorsa Terminal'de şunu çalıştırıp OBSEDRA'yı yeniden aç:

```
xattr -dr com.apple.quarantine /Applications/OBSEDRA.app
```

## Gerekenler
- macOS 11 ya da üstü
- [Claude Code](https://docs.claude.com/en/docs/claude-code) kurulu ve giriş yapılmış olmalı; ajanlar onunla çalışır.

Uygulama boş başlar: projeni, bölgelerini ve ajanlarını sen kurarsın. Verilerin yalnız kendi bilgisayarında, `~/.obsedra` altında durur; ofis ağa açılmaz (yalnız `127.0.0.1`).
