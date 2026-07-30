# Batı Sonrası Dünya — Astro sitesi

Bu klasör GitHub Pages üzerinde çalışacak hazır başlangıç sitesidir.

## En kolay yayınlama yolu

1. GitHub'da `batisonrasi` adında **Public** bir repository açın.
2. Bu zip dosyasını bilgisayarınızda açın.
3. Repository sayfasında **Add file → Upload files** seçin.
4. Zip'in kendisini değil, zip içindeki bütün dosya ve klasörleri yükleyin.
5. **Commit changes** düğmesine basın.
6. GitHub'da **Settings → Pages → Source → GitHub Actions** seçin.
7. **Actions** sekmesinde yayın işleminin yeşil tik olmasını bekleyin.

## Yayından önce değiştirilecek yerler

Projede `SATIN_ALMA_LINKI` yazısını aratın ve gerçek satış bağlantısıyla değiştirin.

Düzenlenecek başlıca dosyalar:

- `src/layouts/Base.astro`
- `src/pages/index.astro`
- `src/pages/kitap.astro`
- `src/pages/kunye.astro`

## Alan adı

`public/CNAME` dosyasında `www.batisonrasi.com` yazıyor.

Alan adı sağlayıcısında GitHub Pages DNS kayıtlarını kurduktan sonra GitHub'da:

Settings → Pages → Custom domain → `www.batisonrasi.com`

## Yeni yazı ekleme

1. PDF'yi `public/yazilar/` klasörüne yükleyin.
2. `src/data/posts.js` dosyasına yeni yazının bilgilerini ekleyin.
3. `src/pages/yazilar/` içinde yeni bir `.astro` sayfası oluşturun.
4. Değişiklikleri commit edin; site otomatik yayınlanır.

## Bilgisayarda önizleme

Node.js kuruluysa:

```bash
npm install
npm run dev
```

Tarayıcıda `http://localhost:4321` adresini açın.
