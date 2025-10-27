# 📊 คู่มือ SEO - ร้านพร้อมพาณิชย์

คู่มือนี้จะช่วยให้ร้านพร้อมพาณิชย์ถูกค้นหาเจอบน Google และ Social Media ได้ง่ายขึ้น

---

## ✅ สิ่งที่ติดตั้งแล้ว

### 1. 🏷️ Meta Tags (SEO พื้นฐาน)
- ✅ Title Tag - หัวข้อที่แสดงบน Google Search
- ✅ Meta Description - คำอธิบายที่แสดงใต้ลิงก์
- ✅ Keywords - คำค้นหาที่เกี่ยวข้อง
- ✅ Robots Meta - บอก Google ให้ index หน้านี้
- ✅ Language - ระบุเป็นภาษาไทย
- ✅ Theme Color - สีของ browser bar บนมือถือ

### 2. 📱 Open Graph (Social Media)
- ✅ Facebook Sharing - เวลาแชร์บน Facebook จะแสดงสวยงาม
- ✅ Twitter Card - แสดงผลบน Twitter
- ✅ Business Contact Data - ข้อมูลธุรกิจ
- ✅ Location Data - พิกัด GPS

### 3. 🏪 Structured Data (JSON-LD)
- ✅ LocalBusiness Schema - บอก Google ว่าเป็นธุรกิจท้องถิ่น
- ✅ Opening Hours - เวลาเปิด-ปิด
- ✅ Address - ที่อยู่
- ✅ GPS Coordinates - พิกัด
- ✅ Rating - คะแนนรีวิว
- ✅ BreadcrumbList - เส้นทางนำทาง

### 4. 🗺️ Sitemap & Robots
- ✅ `sitemap.xml` - แผนที่เว็บไซต์
- ✅ `robots.txt` - กำหนดให้ Google เข้าถึงได้

---

## 📝 สิ่งที่ต้องแก้ไขให้ตรงกับร้านจริง

### 1. เปลี่ยน URL ทั้งหมด
ค้นหาและแทนที่ `https://yourdomain.github.io/` ด้วย URL จริงของคุณ:

**ไฟล์ที่ต้องแก้:**
- [ ] `index.html` - ทุกที่ที่เจอ
- [ ] `sitemap.xml` - แก้ทุก URL
- [ ] `robots.txt` - บรรทัด Sitemap

### 2. เปลี่ยนเบอร์โทรศัพท์
ค้นหาและแทนที่:
- `08x-xxx-xxxx` → เบอร์จริง (เช่น `081-234-5678`)
- `+66-8x-xxx-xxxx` → `+66-81-234-5678`

**ไฟล์ที่ต้องแก้:**
- [ ] `index.html` - ทั้ง meta tags และเนื้อหา

### 3. ปรับพิกัด GPS ให้ตรง
ค้นหาและแทนที่:
- Latitude: `15.481751` → พิกัดจริง
- Longitude: `103.879009` → พิกัดจริง

**วิธีหาพิกัดจริง:**
1. เปิด Google Maps
2. คลิกขวาที่ตำแหน่งร้าน
3. คัดลอกพิกัด (เช่น 15.481751, 103.879009)

**ไฟล์ที่ต้องแก้:**
- [ ] `index.html` - ใน JSON-LD และ JavaScript

### 4. อัพโหลดรูปภาพ
ให้แน่ใจว่ามีไฟล์เหล่านี้:

```
assets/
├── logo.svg              # โลโก้ร้าน (SVG)
├── favicon.png           # ไอคอนเว็บ 32x32px
├── apple-touch-icon.png  # ไอคอน iOS 180x180px
├── storefront.jpg        # รูปหน้าร้าน (1200x630px แนะนำ)
└── 360/
    └── interior.jpg      # รูป 360° ภายในร้าน
```

**ขนาดแนะนำ:**
- `storefront.jpg` - 1200x630px (สำหรับ Open Graph)
- `logo.svg` - Vector ขนาดไหนก็ได้
- `favicon.png` - 32x32px หรือ 192x192px
- `apple-touch-icon.png` - 180x180px

---

## 🚀 ขั้นตอนหลังจาก Deploy

### 1. ส่ง Sitemap ให้ Google
1. ไปที่ [Google Search Console](https://search.google.com/search-console)
2. เพิ่มเว็บไซต์ของคุณ
3. ไปที่ Sitemaps > Add new sitemap
4. ใส่ `https://yourdomain.github.io/sitemap.xml`

### 2. ตรวจสอบ Structured Data
1. ไปที่ [Rich Results Test](https://search.google.com/test/rich-results)
2. ใส่ URL ของคุณ
3. ตรวจสอบว่าผ่านทุกข้อหรือไม่

### 3. ทดสอบ Open Graph
1. ไปที่ [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/)
2. ใส่ URL ของคุณ
3. กด "Scrape Again" เพื่อให้ Facebook อัพเดตข้อมูล

### 4. ลงทะเบียน Google My Business
1. ไปที่ [Google My Business](https://www.google.com/business/)
2. เพิ่มธุรกิจของคุณ
3. กรอกข้อมูล:
   - ชื่อร้าน: ร้านพร้อมพาณิชย์
   - ประเภท: ร้านชำ / Convenience Store
   - ที่อยู่: ใกล้ อบต.ท่าหาดยาว จ.ร้อยเอ็ด
   - เบอร์โทร: 08x-xxx-xxxx
   - เวลาทำการ: 06:00 - 22:00 (ทุกวัน)
   - เว็บไซต์: https://yourdomain.github.io/

---

## 🔍 คำค้นหาที่ควรอันดับได้

จากการตั้งค่า SEO ที่ทำไว้ ร้านควรถูกค้นหาเจอจากคำเหล่านี้:

### คำค้นหาหลัก:
- ✅ ร้านพร้อมพาณิชย์
- ✅ ร้านชำร้อยเอ็ด
- ✅ ร้านชำท่าหาดยาว
- ✅ ร้านสะดวกซื้อร้อยเอ็ด

### คำค้นหาตามทำเล:
- ✅ ร้านค้าใกล้ อบต.ท่าหาดยาว
- ✅ ร้านชำใกล้ฉัน (ถ้ามีการค้นหาแบบ location-based)
- ✅ ร้านค้าใกล้ร้านไอศวรรย์วัสดุ

### คำค้นหาตามสินค้า:
- ✅ ข้าวสารร้อยเอ็ด
- ✅ ของใช้ประจำวันร้อยเอ็ด
- ✅ ร้านขายของชำร้อยเอ็ด

---

## 📈 ติดตามผลลัพธ์

### Google Analytics (แนะนำ)
เพิ่ม tracking code เพื่อดูสถิติผู้เข้าชม:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### ข้อมูลที่ควรติดตาม:
- จำนวนผู้เข้าชมต่อวัน
- คำค้นหาที่พบเว็บไซต์
- หน้าที่ผู้ใช้ดูนานที่สุด
- อัตราการคลิกโทรศัพท์

---

## ✨ Tips เพิ่มเติม

### 1. เพิ่มเนื้อหาเป็นประจำ
- โพสต์โปรโมชั่นใหม่ทุกสัปดาห์
- อัพเดตรูปภาพสินค้าใหม่
- เพิ่มบทความ "สินค้าแนะนำ"

### 2. รีวิวจากลูกค้า
- ขอให้ลูกค้ารีวิวบน Google Maps
- แชร์รีวิวดีๆ บนเว็บไซต์
- ตอบรีวิวทุกรีวิว (ดีหรือไม่ดี)

### 3. Social Media Integration
- แชร์ลิงก์เว็บไซต์บน Facebook
- ใส่ลิงก์ใน LINE OA
- QR Code สำหรับแสกนดูเว็บ

### 4. Local SEO
- ลงทะเบียน Google My Business
- เพิ่มร้านใน LINE Place
- ลงทะเบียนใน Wongnai (ถ้าเหมาะสม)

---

## 🆘 แก้ไขปัญหา SEO

### ปัญหา: ไม่ขึ้นใน Google Search
**วิธีแก้:**
1. ตรวจสอบว่า deploy แล้วหรือยัง
2. ส่ง sitemap ใน Google Search Console
3. รอ 1-2 สัปดาห์ให้ Google index
4. ตรวจสอบ robots.txt ว่าไม่ได้บล็อก Google

### ปัญหา: รูปไม่แสดงเวลาแชร์
**วิธีแก้:**
1. ตรวจสอบว่ารูปอัพโหลดแล้ว
2. URL ของรูปต้องเป็น absolute path (https://...)
3. รูปต้องมีขนาดไม่เกิน 5MB
4. ใช้ Facebook Debugger Scrape Again

### ปัญหา: Structured Data Error
**วิธีแก้:**
1. ใช้ Rich Results Test ตรวจสอบ
2. แก้ syntax error ใน JSON-LD
3. ตรวจสอบว่าข้อมูลครบถ้วน

---

## 📞 ติดต่อขอความช่วยเหลือ

หากมีปัญหาเกี่ยวกับ SEO สามารถ:
- Google "วิธีทำ SEO ร้านค้า"
- ดู YouTube "Local SEO for small business"
- ใช้ Google Search Console Help

---

**อัพเดตล่าสุด:** 2025-01-28
**สถานะ:** ✅ พร้อมใช้งาน
