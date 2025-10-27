# 🚀 คู่มือ Deploy ขึ้น GitHub Pages

คู่มือนี้จะสอนวิธี deploy เว็บไซต์ร้านพร้อมพาณิชย์ขึ้น GitHub Pages **ฟรี!**

---

## 📋 สิ่งที่ต้องเตรียม

- ✅ บัญชี GitHub (ถ้ายังไม่มี สมัครที่ https://github.com)
- ✅ Git ติดตั้งในเครื่อง (ดาวน์โหลดที่ https://git-scm.com)
- ✅ โฟลเดอร์ web-me ที่มีไฟล์ทั้งหมด

---

## 🎯 ขั้นตอนที่ 1: สร้าง Repository บน GitHub

### 1.1 เข้าสู่ GitHub
1. เปิด https://github.com
2. กด **Sign in** (หรือ **Sign up** ถ้ายังไม่มีบัญชี)

### 1.2 สร้าง Repository ใหม่
1. กดปุ่ม **+** มุมบนขวา → เลือก **New repository**
2. กรอกข้อมูล:
   - **Repository name:** `web-me` (หรือชื่ออื่นที่ต้องการ)
   - **Description:** "ร้านพร้อมพาณิชย์ - Landing Page"
   - เลือก **Public** (สำคัญ! ต้อง Public ถึงจะใช้ GitHub Pages ฟรีได้)
   - ❌ **อย่า**ติ๊ก "Add a README file"
   - ❌ **อย่า**เลือก .gitignore
   - ❌ **อย่า**เลือก license
3. กด **Create repository**

### 1.3 คัดลอก URL ของ Repository
หลังสร้างเสร็จจะเห็นหน้าต่างแนะนำ ให้สังเกต URL แบบนี้:
```
https://github.com/USERNAME/web-me.git
```
**คัดลอก URL นี้ไว้**

---

## 🎯 ขั้นตอนที่ 2: เตรียมไฟล์สำหรับ Deploy

### 2.1 สร้าง .gitignore
สร้างไฟล์ `.gitignore` ในโฟลเดอร์ `web-me`:

```
# ไฟล์ที่ไม่ต้อง commit
.DS_Store
Thumbs.db
*.log
node_modules/
.vscode/
.idea/
*.swp
*.swo
*~
```

### 2.2 ตรวจสอบไฟล์ทั้งหมด
ให้แน่ใจว่าโฟลเดอร์ `web-me` มีไฟล์เหล่านี้:
```
web-me/
├── index.html           ✅
├── styles.css           ✅
├── sitemap.xml          ✅
├── robots.txt           ✅
├── .gitignore           ✅ (สร้างใหม่)
├── SEO-GUIDE.md         ✅
├── DEPLOY-GUIDE.md      ✅
└── assets/              (สร้างถ้ายังไม่มี)
    ├── logo.svg
    ├── favicon.png
    ├── apple-touch-icon.png
    ├── storefront.jpg
    └── 360/
        └── interior.jpg
```

---

## 🎯 ขั้นตอนที่ 3: Push Code ขึ้น GitHub

### 3.1 เปิด Terminal/Command Prompt
**Windows:**
- กด `Win + R` → พิมพ์ `cmd` → Enter
- หรือเปิด **Git Bash** (ถ้าติดตั้งแล้ว)

**Mac/Linux:**
- เปิด **Terminal**

### 3.2 เข้าสู่โฟลเดอร์ web-me
```bash
cd e:\ระบบ-pos\web-me
```

### 3.3 ตรวจสอบว่าอยู่ในโฟลเดอร์ที่ถูกต้อง
```bash
dir    # Windows
ls     # Mac/Linux
```
ต้องเห็นไฟล์ `index.html`, `styles.css` ฯลฯ

### 3.4 เริ่มต้น Git Repository
```bash
git init
```
ผลลัพธ์: `Initialized empty Git repository in...`

### 3.5 กำหนดชื่อและอีเมล (ถ้ายังไม่เคยทำ)
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
**แทนที่:**
- `"Your Name"` → ชื่อจริงของคุณ
- `"your.email@example.com"` → อีเมล GitHub ของคุณ

### 3.6 เพิ่มไฟล์ทั้งหมดเข้า Git
```bash
git add .
```

### 3.7 Commit ครั้งแรก
```bash
git commit -m "Initial commit: ร้านพร้อมพาณิชย์ Landing Page"
```

### 3.8 เชื่อมต่อกับ GitHub Repository
```bash
git remote add origin https://github.com/USERNAME/web-me.git
```
**⚠️ สำคัญ:** แทนที่ `USERNAME` ด้วย username GitHub ของคุณ

### 3.9 Push code ขึ้น GitHub
```bash
git branch -M main
git push -u origin main
```

**ถ้าถามรหัสผ่าน:**
- Username: username GitHub ของคุณ
- Password: **Personal Access Token** (ไม่ใช่รหัสผ่านปกติ)

**วิธีสร้าง Personal Access Token:**
1. ไปที่ GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. กด **Generate new token (classic)**
3. ใส่ชื่อ: "Web Deploy"
4. เลือก **repo** (ทั้งหมด)
5. กด **Generate token**
6. **คัดลอก token** (จะไม่แสดงอีก!)
7. วางเป็น password เวลา push

---

## 🎯 ขั้นตอนที่ 4: เปิดใช้งาน GitHub Pages

### 4.1 ไปที่ Repository Settings
1. ไปที่ https://github.com/USERNAME/web-me
2. กดแท็บ **Settings** (มุมบนขวา)

### 4.2 เปิดใช้ GitHub Pages
1. เลื่อนลงไปที่เมนู **Pages** (ซ้ายมือ)
2. ใน **Source** เลือก:
   - Branch: `main`
   - Folder: `/ (root)`
3. กด **Save**

### 4.3 รอสักครู่
- GitHub จะ build และ deploy (ประมาณ 1-2 นาที)
- รีเฟรชหน้าเพื่อดู URL

### 4.4 คัดลอก URL เว็บไซต์
จะเห็นข้อความ:
```
Your site is live at https://USERNAME.github.io/web-me/
```
**✅ นี่คือ URL เว็บไซต์ของคุณ!**

---

## 🎯 ขั้นตอนที่ 5: อัปเดต URL ในไฟล์

### 5.1 แทนที่ URL ทั้งหมด
เปิดไฟล์เหล่านี้และแทนที่:

**ค้นหา:**
```
https://yourdomain.github.io/
```

**แทนที่ด้วย:**
```
https://USERNAME.github.io/web-me/
```

**ไฟล์ที่ต้องแก้:**
- ✅ `index.html` (ทุกที่ที่เจอ - มี 10+ แห่ง)
- ✅ `sitemap.xml` (ทุก URL)
- ✅ `robots.txt` (บรรทัด Sitemap)

### 5.2 Commit และ Push การเปลี่ยนแปลง
```bash
git add .
git commit -m "Update URLs to GitHub Pages domain"
git push
```

### 5.3 รอ 1-2 นาที
GitHub Pages จะ rebuild อัตโนมัติ

---

## 🎯 ขั้นตอนที่ 6: ทดสอบเว็บไซต์

### 6.1 เปิดเว็บไซต์
เปิด: `https://USERNAME.github.io/web-me/`

### 6.2 ตรวจสอบ
- ✅ หน้าเว็บโหลดได้ไหม
- ✅ CSS โหลดถูกต้องไหม
- ✅ รูปภาพแสดงผลไหม (ถ้ามี)
- ✅ แผนที่แสดงไหม
- ✅ 360 viewer ทำงานไหม (ถ้ามีรูป)

### 6.3 ทดสอบบนมือถือ
เปิด URL บนมือถือ ตรวจสอบ:
- ✅ Responsive design
- ✅ ปุ่มโทรศัพท์คลิกได้ไหม

---

## 🎯 ขั้นตอนที่ 7: SEO Setup หลัง Deploy

### 7.1 ส่ง Sitemap ให้ Google
1. ไปที่ https://search.google.com/search-console
2. กด **Add property**
3. เลือก **URL prefix**
4. ใส่: `https://USERNAME.github.io/web-me/`
5. ยืนยันความเป็นเจ้าของ (ใช้วิธี HTML tag)
6. ไปที่ **Sitemaps** → Add new sitemap
7. ใส่: `sitemap.xml`
8. กด **Submit**

### 7.2 ทดสอบ Rich Results
1. ไปที่ https://search.google.com/test/rich-results
2. ใส่ URL: `https://USERNAME.github.io/web-me/`
3. กด **Test URL**
4. ตรวจสอบว่า LocalBusiness schema ถูกต้อง

### 7.3 ทดสอบ Facebook Sharing
1. ไปที่ https://developers.facebook.com/tools/debug/
2. ใส่ URL เว็บไซต์
3. กด **Scrape Again**
4. ตรวจสอบ preview

---

## 📝 วิธีอัปเดตเว็บไซต์ (ครั้งต่อๆ ไป)

เมื่อต้องการแก้ไขเว็บไซต์:

### 1. แก้ไขไฟล์ในเครื่อง
แก้ `index.html`, `styles.css` หรือไฟล์อื่นๆ

### 2. ทดสอบในเครื่อง
เปิดไฟล์ `index.html` ในเบราว์เซอร์

### 3. Commit และ Push
```bash
git add .
git commit -m "อธิบายการเปลี่ยนแปลง"
git push
```

### 4. รอ 1-2 นาที
เว็บไซต์จะอัปเดตอัตโนมัติ

---

## 🎨 Custom Domain (ถ้าต้องการ)

### ถ้าต้องการใช้ชื่อโดเมนของตัวเอง (เช่น `www.promphapanit.com`)

### 1. ซื้อโดเมน
จาก:
- Namecheap
- GoDaddy
- CloudFlare (ถูกสุด)

### 2. ตั้งค่า DNS
เพิ่ม CNAME Record:
```
Type:  CNAME
Name:  www
Value: USERNAME.github.io
```

### 3. ตั้งค่าใน GitHub
1. ไปที่ Repository → Settings → Pages
2. ใน **Custom domain** ใส่: `www.promphapanit.com`
3. กด **Save**
4. รอ DNS propagate (5-30 นาที)

---

## ❗ แก้ปัญหาที่พบบ่อย

### ปัญหา: หน้าเว็บขึ้น 404 Not Found
**วิธีแก้:**
1. ตรวจสอบว่า GitHub Pages เปิดอยู่ไหม
2. ตรวจสอบ Branch เป็น `main` หรือไม่
3. ตรวจสอบว่าไฟล์ชื่อ `index.html` (ตัวพิมพ์เล็ก)
4. รอ 2-3 นาทีแล้วรีเฟรช

### ปัญหา: CSS/รูปภาพไม่โหลด
**วิธีแก้:**
1. เปิด DevTools (F12) → Console
2. ดูว่ามี error อะไร
3. ตรวจสอบ path ของไฟล์ (ต้องเป็น relative path)
4. **ถ้าใช้ subfolder** เช่น `/web-me/` ต้องแก้ path:
   - ❌ `href="/styles.css"`
   - ✅ `href="./styles.css"` หรือ `href="styles.css"`

### ปัญหา: git push ไม่ได้
**วิธีแก้:**
```bash
# ถ้า rejected
git pull origin main --rebase
git push

# ถ้าต้องการบังคับ (ระวัง! จะลบ history)
git push -f origin main
```

### ปัญหา: ลืม Personal Access Token
**วิธีแก้:**
1. ไปที่ GitHub → Settings → Developer settings → Personal access tokens
2. สร้าง token ใหม่
3. เก็บไว้ในที่ปลอดภัย

---

## 🎉 เสร็จสิ้น!

เว็บไซต์ของคุณตอนนี้:
- ✅ Deploy บน GitHub Pages (ฟรี!)
- ✅ มี URL สาธารณะ
- ✅ SSL/HTTPS อัตโนมัติ
- ✅ พร้อม SEO
- ✅ พร้อม deploy ทุกครั้งที่ push

---

## 📞 ติดต่อขอความช่วยเหลือ

- **GitHub Docs:** https://docs.github.com/pages
- **Git Tutorial:** https://git-scm.com/book/th/v2
- **YouTube:** ค้นหา "GitHub Pages tutorial"

---

**สร้างเมื่อ:** 2025-01-28
**สถานะ:** ✅ พร้อมใช้งาน
