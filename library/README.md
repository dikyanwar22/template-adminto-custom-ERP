# Library — Adminto Template (Isolated)

Folder ini **terisolasi** dari `assets/` milik `ERP.html`. Tujuannya agar tidak tabrakan.

```
library/  (sejajar dengan ERP.html)
├── css/
│   └── style.css   ← copy dari assets/css/style.css (isolated)
├── js/
│   └── main.js     ← copy dari assets/js/main.js (isolated)
├── index.html      ← katalog preview semua template (buka ini dulu) — sejajar dengan menu-menu
├── 01-blank.html              ← starter kosong, paling bersih
├── 02-cards-widgets.html      ← cards & stat widgets
├── 03-tables.html             ← 4 variasi tabel (basic)
├── 04-forms.html              ← forms basic + validation
├── 05-charts.html             ← ApexCharts (area, donut, bar, line)
├── 06-ui-elements.html        ← buttons, badges, alerts, tabs, modals
├── 07-starter-full-erp.html   ← duplikat menu lengkap ERP.html (rekomendasi)
├── 08-datatables.html         ← DataTables 1.13 + Buttons Excel/PDF/Print
├── 09-calendar.html           ← FullCalendar 6.1 drag & drop
├── 10-form-advanced.html      ← flatpickr, Tom Select, dropzone, wizard
└── 11-apps.html               ← kanban, chat, timeline, file manager
```

## Cara Pakai (Copy-Paste)

1. Buka `library/index.html` untuk melihat katalog (semua menu sejajar di folder yang sama).
2. Pilih salah satu file di `library/` misal `08-datatables.html` dan **copy file** tersebut.
3. Paste jadi file baru, misal `penjualan.html` atau `master-produk.html`.
4. Edit hanya bagian `.main-content` — header/topnav/drawer sudah siap.
5. **Penting path asset:**
   - Jika file tetap di `library/` → biarkan `css/style.css` & `js/main.js`
   - Jika file baru di root (sejajar `ERP.html`) → ganti menjadi `library/css/style.css` & `library/js/main.js`
6. Untuk menambah submenu, copy blok `dropdown-submenu` dari `ERP.html` baris 40–60.

## Kenapa Isolated?

- `ERP.html` tetap memakai `assets/css/style.css` & `assets/js/main.js` via CDN + lokal.
- Semua template di `library/` memakai `library/css/style.css` & `library/js/main.js` sendiri.
- Jadi edit di `library/` tidak akan merusak `ERP.html`, dan sebaliknya.

## Versi

- Bootstrap 5.3.3 (CDN)
- RemixIcon 4.2.0 + Bootstrap Icons 1.11.3
- DataTables 1.13 + FullCalendar 6.1 + flatpickr + Tom Select
- ApexCharts (CDN) untuk charts
- Font: Nunito + Poppins
