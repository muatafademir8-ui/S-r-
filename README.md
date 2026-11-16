# Açık Dünya Sürüş – PSP Edition (ilk port prototipi)

Bu klasör, yüklediğin `Açık Dünya Sürüş.html` oyununun PSP için yeniden yazılmaya başlanmış C/PSP-GU prototipidir.

## Bu ilk sürümde
- PSP GU ile gerçek 3D perspektif çizimi
- Sonsuz ızgara şehir yaklaşımı ve prosedürel binalar
- Takip kamerası ve Tesla tarzı oyuncu aracı
- Gaz, fren, direksiyon, nitro ve drift girdileri
- Basit trafik görselleştirmesi
- Hız / nitro / çarpışma bilgi ekranı

## Kontroller
- X veya Yukarı: Gaz
- Kare veya Aşağı: Fren / geri
- Sol / Sağ: Direksiyon
- L / R: Direksiyon
- O: Nitro
- Üçgen: Drift
- START: Çıkış

## Derleme
Bu kaynak kodu tek başına EBOOT.PBP değildir. EBOOT.PBP üretmek için PSP homebrew geliştirme ortamı (PSPSDK) gerekir.

PSPSDK kurulu bir ortamda bu klasörde:
```sh
make
```
komutunu çalıştır. Başarılı derlemede `EBOOT.PBP` oluşur. PSP hafıza kartında:
`/PSP/GAME/AcikDunyaSurus/EBOOT.PBP`
yoluna koyabilirsin. Önce PPSSPP'de test etmen önerilir.

## Dürüst durum notu
Bu bir ilk oynanabilir port iskeletidir; HTML sürümündeki Three.js kodunun birebir ve eksiksiz karşılığı değildir. İlk aşamada şehir, araç, takip kamerası ve temel sürüş oluşturuldu. Orijinal oyundaki gerçek trafik yapay zekâsı, çarpışınca araçların uçması, bina parçalanması, altınların fiziksel toplanması, mini harita, ses ve tam HUD sonraki geliştirme adımlarıdır. PSP donanımına göre poligon ve çizim optimizasyonu da gerekecektir.
