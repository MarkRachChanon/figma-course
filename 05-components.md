# 5. Components & Design System

[← ก่อนหน้า: Design Fundamentals](04-design-fundamentals.md) | [หน้าหลัก](README.md) | [ถัดไป: Prototyping →](06-prototyping.md)

---

## 🎯 จุดประสงค์การเรียนรู้

- สร้างและใช้งาน Components ได้
- เข้าใจ Design System และประโยชน์
- สร้าง Components ที่ใช้ซ้ำได้ (Button, Input, Card)
- ติดตั้งและใช้งาน Plugins

---

## a. Create Component

### Component คืออะไร

**คำนิยาม:**
- วัตถุที่สร้างขึ้นเพื่อใช้ซ้ำได้หลายครั้ง
- แก้ Master → Instance ทุกตัวเปลี่ยนตาม

**ข้อดี:**
- ✅ ประหยัดเวลา (ไม่ต้องวาดซ้ำ)
- ✅ สม่ำเสมอ (ดีไซน์เหมือนกันทั้งหมด)
- ✅ ง่ายต่อการแก้ไข (แก้ครั้งเดียวเปลี่ยนทั้งหมด)
- ✅ ทำงานเป็นทีม (แชร์ Component ได้)

### การสร้าง Component

**ขั้นตอน:**
1. วาดวัตถุที่ต้องการ (เช่น ปุ่ม)
2. คลิกขวา → **Create Component**
3. หรือกด `Ctrl/Cmd + Alt + K`
4. ตั้งชื่อ Component

**การตั้งชื่อ:**
ใช้ Slash (/) เพื่อจัดหมวดหมู่:
```
Button/
  Primary
  Secondary
  Outline
  
Icon/
  Home
  User
  Settings
  
Form/
  Input
  Textarea
  Select
```

### การใช้งาน Component

**สร้าง Instance:**
1. Drag Component จาก Assets Panel (ซ้ายมือ)
2. หรือกด `Ctrl/Cmd + Alt + C`

**แก้ไข Master:**
1. คลิกขวาที่ Instance → Go to Main Component
2. แก้ไข Master
3. Instance ทั้งหมดเปลี่ยนตาม

**Override (แก้ไข Instance แยก):**
- เปลี่ยนข้อความได้
- เปลี่ยนสี ขนาดได้
- โครงสร้างยังเชื่อมกับ Master

**Detach Instance:**
- คลิกขวา → Detach Instance
- ตัดการเชื่อมกับ Master
- กลายเป็นวัตถุธรรมดา
- ไม่แนะนำนอกจากจำเป็น

---

## b. Design System

### Design System คืออะไร

**คำนิยาม:**
ชุดของ Components, Styles, Guidelines และ Principles ที่ใช้สร้างความสม่ำเสมอในการออกแบบทั้งองค์กร

### ประกอบด้วย

**1. Color Styles**
- ชุดสีที่กำหนดไว้
- Primary, Secondary, Neutral
- Semantic Colors (Success, Error, Warning)

**2. Text Styles**
- รูปแบบข้อความ
- Heading: H1, H2, H3, H4
- Body: Large, Regular, Small
- Caption, Button Text

**3. Components Library**
- Button (ปุ่ม)
- Form (แบบฟอร์ม)
- Card (การ์ด)
- Navigation
- Modal, Dialog

**4. Grid System**
- Layout Guidelines
- Spacing System (8px grid)
- Responsive Breakpoints

**5. Guidelines**
- เอกสารหลักการใช้งาน
- Do's and Don'ts
- Best Practices

### การสร้าง Styles

**Color Style:**
1. สร้างรูปร่าง (Rectangle)
2. เลือกสีที่ต้องการ
3. คลิก Style icon → Create Style
4. ตั้งชื่อ: `Colors/Primary/500`

**Text Style:**
1. สร้างข้อความ
2. ตั้งค่า Font, Size, Line Height
3. คลิก Text styles → Create Style
4. ตั้งชื่อ: `Typography/H1`

---

## c. Reusable Components

### 1. Button Component

**โครงสร้าง:**
```
[Frame] Button (Auto Layout, Horizontal)
  └─ [Icon] Icon (Optional)
  └─ [Text] Label
```

**การสร้าง:**
1. สร้าง Frame → กด `Shift + A`
2. Direction: Horizontal
3. Padding: 16px (L/R), 12px (T/B)
4. Spacing: 8px (ระหว่าง Icon กับ Text)
5. Corner Radius: 8px
6. Fill: สีหลัก

**Variants:**
- **Types:** Primary, Secondary, Outline, Text
- **States:** Default, Hover, Active, Disabled
- **Sizes:** Small, Medium, Large

**ตัวอย่างการตั้งค่า:**
```
Primary Button (Medium):
- Padding: 16px (L/R), 12px (T/B)
- Font Size: 16px
- Background: #2196F3
- Text Color: #FFFFFF
- Corner Radius: 8px

Secondary Button (Medium):
- Padding: 16px (L/R), 12px (T/B)
- Font Size: 16px
- Background: #E0E0E0
- Text Color: #424242
- Corner Radius: 8px

Disabled Button:
- Opacity: 40%
- Cursor: not-allowed
```

### 2. Input Field Component

**โครงสร้าง:**
```
[Frame] Input Field (Auto Layout, Vertical)
  └─ [Text] Label
  └─ [Frame] Input Container (Auto Layout, Horizontal)
      └─ [Icon] Leading Icon (Optional)
      └─ [Text] Placeholder / Input Text
      └─ [Icon] Trailing Icon (Optional)
  └─ [Text] Helper Text / Error Message
```

**การสร้าง:**
1. สร้าง Frame หลัก (Auto Layout Vertical)
2. Spacing: 8px
3. เพิ่ม Label (Text)
4. เพิ่ม Input Container:
   - Auto Layout Horizontal
   - Padding: 12px
   - Border: 1px #E0E0E0
   - Corner Radius: 8px
   - Background: #FFFFFF
5. เพิ่ม Placeholder Text
6. เพิ่ม Helper Text

**States:**
- Empty: Border #E0E0E0
- Filled: Border #E0E0E0, Text สีดำ
- Focused: Border สีหลัก (2px)
- Error: Border สีแดง, Helper Text สีแดง
- Disabled: Background #F5F5F5, Opacity 50%

### 3. Card Component

**โครงสร้าง:**
```
[Frame] Card (Auto Layout, Vertical)
  └─ [Image] Cover Image
  └─ [Frame] Content (Auto Layout, Vertical)
      └─ [Text] Title (H3)
      └─ [Text] Description (Body)
      └─ [Frame] Footer (Auto Layout, Horizontal)
          └─ [Button] Action Button
          └─ [Icon + Text] Meta Info
```

**การสร้าง:**
1. สร้าง Frame (Auto Layout Vertical)
2. Spacing: 0 (Image ติดกัน)
3. Corner Radius: 12px
4. Drop Shadow: 0px 4px 12px rgba(0,0,0,0.1)
5. เพิ่ม Cover Image (Height: 200px)
6. เพิ่ม Content:
   - Padding: 20px
   - Spacing: 12px
7. เพิ่ม Title, Description
8. เพิ่ม Footer (Space Between)

**Variants:**
- Horizontal Card (Image ซ้าย)
- Vertical Card (Image บน)
- With/Without Image
- With/Without Footer

---

## d. Plugins

### การติดตั้ง Plugins

**วิธีที่ 1: จาก Menu**
1. คลิกเมนู Plugins หรือกด `Ctrl/Cmd + /`
2. เลือก Browse plugins in Community
3. ค้นหา Plugin ที่ต้องการ
4. คลิก Install

**วิธีที่ 2: จาก Community**
1. ไปที่ figma.com/@community
2. เลือก Plugins
3. ค้นหาและติดตั้ง

### Plugin แนะนำ

**1. Iconify** ⭐ สำคัญมาก
- ไอคอนนับแสนตัว
- Icon Sets: Material, Font Awesome, Bootstrap, Feather

**วิธีใช้:**
1. กด `Ctrl/Cmd + /` พิมพ์ "Iconify"
2. ค้นหาไอคอน
3. คลิกเพื่อใส่ใน Canvas
4. ปรับขนาดและสี

**2. Unsplash**
- รูปภาพฟรีคุณภาพสูง

**วิธีใช้:**
1. เปิด Unsplash
2. ค้นหารูปภาพ
3. คลิกเพื่อใส่

**3. Content Reel**
- สร้างข้อมูลตัวอย่าง (Dummy Data)

**ประเภทข้อมูล:**
- ชื่อคน, อีเมล, ที่อยู่
- วันที่, ตัวเลข
- Lorem Ipsum

**วิธีใช้:**
1. เลือก Text Layers
2. เปิด Content Reel
3. เลือกประเภทข้อมูล
4. Apply

**4. Remove BG**
- ลบพื้นหลังรูปภาพ

**วิธีใช้:**
1. เลือกรูปภาพ
2. เปิด Remove BG
3. รอประมวลผล
4. ได้รูปที่ลบพื้นหลัง

**5. Stark**
- ตรวจสอบ Accessibility

**ฟีเจอร์:**
- Contrast Checker
- Color Blind Simulator
- Focus Order

**6. Autoflow**
- สร้างลูกศร Flow อัตโนมัติ

**วิธีใช้:**
1. เลือก 2 Frame
2. เปิด Autoflow
3. คลิก Connect

---

## 💡 Best Practices

**Components:**
- ตั้งชื่อให้เป็นระบบ
- ใช้ Auto Layout เสมอ
- สร้าง Variants สำหรับ States
- อย่าซับซ้อนเกินไป

**Design System:**
- เริ่มจากพื้นฐาน (Colors, Typography)
- สร้าง Components ที่ใช้บ่อย
- Document การใช้งาน
- Update สม่ำเสมอ

**Plugins:**
- ติดตั้งเฉพาะที่จำเป็น
- ทดสอบก่อนใช้งานจริง
- อ่าน Review จากผู้ใช้อื่น

---

## 📝 สรุป

**Components:**
- สร้างด้วย `Ctrl/Cmd + Alt + K`
- ใช้ซ้ำได้ แก้ง่าย
- สร้าง Variants

**Design System:**
- Color Styles + Text Styles
- Components Library
- Guidelines

**Reusable Components:**
- Button (Variants + States)
- Input Field (States)
- Card (Layouts)

**Plugins:**
- Iconify, Unsplash, Content Reel
- Remove BG, Stark, Autoflow

---

[← ก่อนหน้า: Design Fundamentals](04-design-fundamentals.md) | [หน้าหลัก](README.md) | [ถัดไป: Prototyping →](06-prototyping.md)
