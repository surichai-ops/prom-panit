# 🏪 ร้านพร้อมพาณิชย์ - Landing Page

> เว็บไซต์ร้านชำ ใกล้ อบต.ท่าหาดยาว จังหวัดร้อยเอ็ด

[![Deploy Status](https://img.shields.io/badge/status-active-success)](https://github.com/USERNAME/web-me)
[![GitHub Pages](https://img.shields.io/badge/hosted-GitHub%20Pages-blue)](https://USERNAME.github.io/web-me/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

---

## 📋 เกี่ยวกับโปรเจค

Landing page สำหรับร้านพร้อมพาณิชย์ - ร้านชำครบครัน ที่ให้บริการชุมชนใกล้ อบต.ท่าหาดยาว จ.ร้อยเอ็ด

### ✨ Features

- 🗺️ **แผนที่ตำแหน่งร้าน** - OpenStreetMap พร้อม marker
- 🌐 **มุมมอง 360°** - Photo Sphere Viewer สำหรับชมภายในร้าน
- 🎯 **SEO Optimized** - พร้อม meta tags, structured data, sitemap
- 📱 **Responsive Design** - ใช้งานได้ทั้ง desktop และ mobile
- 🎨 **Modern UI** - Gradient, animations, shadows
- 🏷️ **Open Graph** - แชร์บน Facebook/LINE/Twitter สวยงาม

---

## 🛠️ Technology Stack

| Component | Technology |
|-----------|-----------|
| HTML | HTML5 |
| CSS | CSS3 + Custom Properties |
| Maps | Leaflet.js + OpenStreetMap |
| 360° Viewer | Photo Sphere Viewer |
| Language | Thai (ภาษาไทย) |
| Hosting | GitHub Pages |

---

## 🚀 Quick Start

### ดูเว็บไซต์

**🌐 Live Demo:** https://USERNAME.github.io/web-me/

### รันในเครื่อง

```bash
# Clone repository
git clone https://github.com/USERNAME/web-me.git

# เข้าสู่โฟลเดอร์
cd web-me

# เปิดไฟล์ในเบราว์เซอร์
# Windows
start index.html

# Mac
open index.html

# Linux
xdg-open index.html
```

ไม่ต้องติดตั้งอะไร! เปิดไฟล์ `index.html` ใน browser ได้เลย

---

## 📁 โครงสร้างโปรเจค

```
web-me/
├── index.html              # หน้าหลัก
├── styles.css              # Stylesheet หลัก
├── sitemap.xml             # Sitemap สำหรับ SEO
├── robots.txt              # กำหนดการเข้าถึงของ search engines
├── .gitignore              # ไฟล์ที่ไม่ต้อง commit
├── README.md               # คุณกำลังอ่านอยู่
├── SEO-GUIDE.md            # คู่มือ SEO
├── DEPLOY-GUIDE.md         # คู่มือ Deploy
└── assets/                 # รูปภาพและไฟล์สื่อ
    ├── logo.svg            # โลโก้ร้าน
    ├── favicon.png         # Favicon
    ├── apple-touch-icon.png # iOS icon
    ├── storefront.jpg      # รูปหน้าร้าน
    └── 360/
        └── interior.jpg    # รูปพาโนรามา 360°
```

---

## 📖 Documentation

- 📊 **[SEO Guide](SEO-GUIDE.md)** - คู่มือ SEO ฉบับสมบูรณ์
- 🚀 **[Deploy Guide](DEPLOY-GUIDE.md)** - วิธี deploy ขึ้น GitHub Pages

---

## 🎯 SEO Features

### Meta Tags
- ✅ Title, Description, Keywords
- ✅ Open Graph (Facebook, LINE)
- ✅ Twitter Card
- ✅ Robots meta
- ✅ Canonical URL

### Structured Data (JSON-LD)
- ✅ LocalBusiness Schema
- ✅ Opening Hours
- ✅ Address & GPS
- ✅ BreadcrumbList

### Search Engine
- ✅ sitemap.xml
- ✅ robots.txt
- ✅ Semantic HTML

---

## 📞 ข้อมูลร้าน

- **ชื่อ:** ร้านพร้อมพาณิชย์
- **ที่อยู่:** ใกล้ อบต.ท่าหาดยาว จ.ร้อยเอ็ด
- **จุดสังเกต:** ใกล้ร้านไอศวรรย์วัสดุ
- **เวลาทำการ:** 06:00 - 22:00 น. (ทุกวัน)
- **โทร:** 08x-xxx-xxxx

---

## 🔧 Development

### ข้อกำหนด
- Web browser ที่ทันสมัย (Chrome, Firefox, Safari, Edge)
- Text editor (VS Code แนะนำ)
- Git (สำหรับ version control)

### แก้ไขโค้ด

```bash
# สร้าง branch ใหม่
git checkout -b feature/new-feature

# แก้ไขไฟล์

# Commit
git add .
git commit -m "Add: คำอธิบายการเปลี่ยนแปลง"

# Push
git push origin feature/new-feature
```

### Testing

เปิด `index.html` ในหลายๆ browser:
- ✅ Chrome
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

---

## 🎨 Customization

### เปลี่ยนสีธีม

แก้ไขใน `styles.css`:

```css
:root {
  --bg: #ffffff;
  --fg: #1a2332;
  --accent: #0d1699;        /* สีหลัก */
  --accent-light: #3b4fd8;  /* สีรอง */
  --sky: #6b8fff;           /* สีสว่าง */
  --muted: #64748b;         /* สีข้อความรอง */
}
```

### เปลี่ยนฟอนต์

แก้ไขใน `styles.css`:

```css
body {
  font-family: "Noto Sans Thai", sans-serif; /* เปลี่ยนตรงนี้ */
}
```

---

## 📱 Screenshots

### Desktop
![Desktop View](assets/screenshots/desktop.png)

### Mobile
![Mobile View](assets/screenshots/mobile.png)

### 360° Viewer
![360 Viewer](assets/screenshots/360-viewer.png)

---

## 🤝 Contributing

ยินดีรับ contributions!

1. Fork repository
2. สร้าง feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add: AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. เปิด Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👏 Credits

### Libraries & Tools
- [Leaflet.js](https://leafletjs.com/) - Interactive maps
- [Photo Sphere Viewer](https://photo-sphere-viewer.js.org/) - 360° panorama viewer
- [OpenStreetMap](https://www.openstreetmap.org/) - Map data
- [Noto Sans Thai](https://fonts.google.com/noto/specimen/Noto+Sans+Thai) - Thai web font

### Inspiration
- Modern landing page design
- Local business websites
- Google My Business

---

## 📧 Contact

- **Email:** contact@example.com
- **Website:** https://USERNAME.github.io/web-me/
- **Facebook:** [ร้านพร้อมพาณิชย์](https://facebook.com)
- **LINE:** @promphapanit

---

## 🔄 Changelog

### Version 1.0.0 (2025-01-28)
- ✅ Initial release
- ✅ Responsive landing page
- ✅ Interactive map (Leaflet + OSM)
- ✅ 360° photo viewer
- ✅ SEO optimization
- ✅ Structured data
- ✅ Open Graph tags
- ✅ Sitemap & robots.txt

---

## 🎯 Roadmap

### Version 1.1.0 (เร็วๆ นี้)
- [ ] เพิ่มหน้าสินค้าและราคา
- [ ] ระบบแสดงโปรโมชั่นแบบ real-time
- [ ] Integration กับ LINE OA
- [ ] Google Analytics

### Version 2.0.0 (อนาคต)
- [ ] ระบบสั่งซื้อออนไลน์
- [ ] ระบบจัดการสต็อก
- [ ] Admin dashboard
- [ ] Multi-language support

---

## ⭐ Star History

ถ้าชอบโปรเจคนี้ อย่าลืมกด ⭐ Star ด้วยนะครับ!

---

**Made with ❤️ in Roi Et, Thailand**

**© 2025 ร้านพร้อมพาณิชย์ - All Rights Reserved**
