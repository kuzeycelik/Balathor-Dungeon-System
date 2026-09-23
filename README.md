# Balathor'un Mahzeni

Metin2 Balathor sistemi icin kaynak, client pack ve server dosyalari. Verilen paket, GitHub'daki `Official Community System` ornegindeki dizilime gore ayrildi. Kod ve varlik dosyalarinin icerigi degistirilmedi.

## Klasor yapisi

```text
01. Svn/
  Client/       Client C++ kaynak dosyalari
  Server/       Game, DB ve common kaynak dosyalari
02. Client/     Pack varliklari: root, locale, uiscript, map, effect, monster2 ...
03. Server/     share/locale/turkey ve proto verileri
```

## Kurulum

1. `01. Svn` dosyalarini kendi source agacinizla karsilastirip birlestirin. Mevcut dosyalari topluca uzerine yazmayin.
2. `02. Client` icindeki klasorleri ilgili client pack hedeflerine birlestirin.
3. `03. Server` icindeki map, monster, quest ve proto verilerini mevcut server dizinleriyle birlestirin.
4. `01. Svn/Server/game/MakeFile` yalnizca kaynak dosyasi adlarini iceren bir parcadir. Bunlari kendi build dosyaniza ekleyin.
5. Quest fonksiyon kayitlarini, map index/config kaydini, vnum cakismalarini ve client-server packet uyumunu kendi fork'unuzda dogrulayin.

## Notlar

- Paket 1.882 dosya icerir: 1.724 client, 100 server ve 58 source dosyasi.
- Bazi efekt ve camera varliklari diger sistemlerle ortak olabilir; verilen paketten cikarilmadi.
- [Metin2 Wiki Balathor sayfasi](https://tr-wiki.metin2.gameforge.com/index.php/Balathor%27un_Mahzeni) oynanis referansidir. Resmi sistemle birebir uyumluluk bu depoda test edilmedi.
- Pakette lisans belgesi bulunmuyor. Kamuya acik yayindan once dosyalarin dagitim haklarini dogrulayin.