# 📁 Assets Folder

โฟลเดอร์นี้เก็บรูปภาพและไฟล์สื่อต่างๆ สำหรับเว็บไซต์

---

## 📋 ไฟล์ที่ต้องมี

### 1. โลโก้ร้าน
**ไฟล์:** `logo.svg`
- **ขนาด:** ไม่จำกัด (SVG เป็น vector)
- **คำแนะนำ:** ออกแบบโลโก้ที่สื่อความหมายของร้าน
- **ตัวอย่าง:** ใช้ Canva, Figma, หรือ Adobe Illustrator

### 2. Favicon
**ไฟล์:** `favicon.png`
- **ขนาด:** 32x32px หรือ 192x192px
- **รูปแบบ:** PNG
- **คำแนะนำ:** ควรเป็นรูปง่ายๆ ที่มองเห็นได้ชัดแม้ขนาดเล็ก

### 3. Apple Touch Icon
**ไฟล์:** `apple-touch-icon.png`
- **ขนาด:** 180x180px
- **รูปแบบ:** PNG
- **คำแนะนำ:** สำหรับผู้ใช้ iOS เมื่อบันทึกเว็บไซต์ไว้ที่ home screen

### 4. รูปหน้าร้าน
**ไฟล์:** `storefront.jpg`
- **ขนาด:** 1200x630px (แนะนำสำหรับ Open Graph)
- **รูปแบบ:** JPG หรือ PNG
- **คำแนะนำ:**
  - ถ่ายให้เห็นหน้าร้านชัดเจน
  - แสงสว่างเพียงพอ
  - ป้ายร้านอ่านได้ชัด
  - ไม่มีรถหรือของกีดขวาง

### 5. รูป 360° ภายในร้าน
**ไฟล์:** `360/interior.jpg`
- **ขนาด:** อย่างน้อย 4096x2048px (equirectangular)
- **รูปแบบ:** JPG
- **คำแนะนำ:**
  - ใช้แอพ Google Street View
  - หรือกล้อง 360° (Ricoh Theta, Insta360)
  - ถ่ายตอนร้านเปิด แสงสว่างดี
  - จัดสินค้าให้เรียบร้อย

---

## 📸 วิธีถ่ายรูปหน้าร้าน

### เคล็ดลับการถ่ายภาพ:
1. **เวลา:** ถ่ายตอนกลางวัน แสงสว่างดี
2. **มุม:** ตั้งตรง ไม่เอียง
3. **ระยะ:** ห่างพอให้เห็นทั้งร้าน
4. **เนื้อหา:** เห็นป้ายร้าน + หน้าบ้าน/ร้านชัดเจน
5. **บรรยากาศ:** ดูน่าเข้า สะอาดเรียบร้อย

### แก้ไขภาพ (ถ้าต้องการ):
- ตัดขอบให้สัดส่วน 1200x630
- ปรับแสงให้สว่างขึ้น
- เพิ่มความคมชัด
- ลดขนาดไฟล์ให้ไม่เกิน 500KB

---

## 🌐 วิธีถ่ายภาพ 360°

### ใช้แอพ Google Street View (ฟรี):

#### 1. ดาวน์โหลดแอพ
- **Android:** Google Play Store
- **iOS:** App Store

#### 2. ถ่ายภาพ
1. เปิดแอพ → กด **+** → เลือก **Camera**
2. ยืนตรงกลางร้าน
3. ถือมือถือให้ตรง
4. หมุนตัวช้าๆ ตามจุดที่แอพบอก
5. ถ่ายครบทุกจุด (ประมาณ 20-30 จุด)

#### 3. ส่งออกภาพ
1. กด **Save**
2. รอประมวลผล
3. กด **Export** → **Save to device**
4. เปลี่ยนชื่อเป็น `interior.jpg`
5. ย้ายไฟล์มาที่ `assets/360/`

---

## 🎨 สร้างโลโก้ฟรี

### ใช้ Canva (แนะนำ):
1. ไปที่ https://www.canva.com
2. เลือก **Logo** template
3. แก้ไข:
   - ชื่อร้าน: "ร้านพร้อมพาณิชย์"
   - สี: น้ำเงิน (#0d1699)
   - ไอคอน: ร้านค้า 🏪
4. Export → SVG (Pro) หรือ PNG

### ใช้ Online Tools อื่นๆ:
- **LogoMaker:** https://logomakr.com
- **Hatchful:** https://hatchful.shopify.com
- **FreeLogoDesign:** https://www.freelogodesign.org

---

## 🖼️ แหล่ง Stock Photos (ถ้าไม่มีรูปจริง)

### รูปหน้าร้านชำ:
- **Unsplash:** https://unsplash.com/s/photos/convenience-store
- **Pexels:** https://www.pexels.com/search/shop/
- **Pixabay:** https://pixabay.com/images/search/store/

### รูป 360° ตัวอย่าง:
- Photo Sphere Viewer demo: https://photo-sphere-viewer.js.org/assets/sphere.jpg

**⚠️ หมายเหตุ:** ใช้รูปจริงของร้านจะดีที่สุด!

---

## ✅ Checklist ก่อน Deploy

- [ ] มี `logo.svg` หรือ `logo.png`
- [ ] มี `favicon.png` (32x32 หรือ 192x192)
- [ ] มี `apple-touch-icon.png` (180x180)
- [ ] มี `storefront.jpg` (1200x630)
- [ ] มี `360/interior.jpg` (ถ้าต้องการ 360 viewer)
- [ ] รูปทุกรูปชัดเจน ไม่เบลอ
- [ ] ขนาดไฟล์ไม่เกิน 1MB ต่อรูป
- [ ] ใช้ชื่อไฟล์ตรงตาม spec

---

## 📏 สรุปขนาดไฟล์

| ไฟล์ | ขนาดแนะนำ | รูปแบบ | ใช้งาน |
|------|-----------|--------|--------|
| `logo.svg` | Vector | SVG | โลโก้หลัก |
| `favicon.png` | 32x32 หรือ 192x192 | PNG | Browser icon |
| `apple-touch-icon.png` | 180x180 | PNG | iOS home screen |
| `storefront.jpg` | 1200x630 | JPG | Open Graph, หน้าเว็บ |
| `360/interior.jpg` | 4096x2048+ | JPG | Photo Sphere Viewer |

---

## 🔧 เครื่องมือแก้ไขรูป

### Online (ฟรี):
- **Photopea:** https://www.photopea.com (เหมือน Photoshop)
- **Pixlr:** https://pixlr.com
- **Canva:** https://www.canva.com

### Desktop:
- **GIMP:** https://www.gimp.org (ฟรี)
- **Paint.NET:** https://www.getpaint.net (Windows, ฟรี)
- **Photoshop:** (เสียเงิน)

### ลดขนาดไฟล์:
- **TinyPNG:** https://tinypng.com
- **Squoosh:** https://squoosh.app

---

**สร้างเมื่อ:** 2025-01-28
**สถานะ:** ✅ พร้อมใช้งาน
