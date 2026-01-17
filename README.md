# เนื้อหาการสอน Figma สำหรับนักศึกษาระดับ ปวส.

ไฟล์นี้จัดทำขึ้นเพื่อใช้เป็นเอกสารประกอบการสอนวิชา Figma  
สำหรับนักศึกษาระดับประกาศนียบัตรวิชาชีพชั้นสูง (ปวส.)

---

## สารบัญ

1. [Introduction (บทนำ)](#1-introduction-บทนำ)
2. [Getting Started (เริ่มต้นใช้งาน)](#2-getting-started-เริ่มต้นใช้งาน)
3. [Basic Tools & Features](#3-basic-tools--features-เครื่องมือและฟีเจอร์พื้นฐาน)
4. [Design Fundamentals](#4-design-fundamentals-หลักการออกแบบ)
5. [Components & Design System](#5-components--design-system)
6. [Prototyping](#6-prototyping-การสร้างต้นแบบ)

---

## 1. Introduction (บทนำ)

### จุดประสงค์การเรียนรู้
- รู้จัก Figma และประโยชน์ในการออกแบบ UI/UX
- เข้าใจความแตกต่างระหว่าง Figma กับโปรแกรมออกแบบอื่นๆ
- ทำความเข้าใจการทำงานแบบ Cloud-based

### Figma คืออะไร
Figma เป็นเครื่องมือออกแบบ UI/UX แบบออนไลน์ที่ใช้งานผ่าน Web Browser หรือ Desktop Application สามารถออกแบบเว็บไซต์ แอปพลิเคชัน และสร้าง Prototype ได้อย่างครบวงจร

### ข้อดีของ Figma
- **ใช้งานผ่าน Browser** - ไม่ต้องติดตั้งโปรแกรมหนัก
- **ทำงานร่วมกันแบบ Real-time** - หลายคนแก้ไขไฟล์เดียวกันพร้อมกันได้
- **ฟรีสำหรับนักเรียน/นักศึกษา** - สามารถใช้งานฟีเจอร์หลักได้ฟรี
- **Community ใหญ่** - มี Template และ Plugin มากมายให้เลือกใช้
- **Cross-platform** - ใช้งานได้ทั้ง Windows, Mac, Linux, Web

### การใช้งาน Figma
- Web Design - ออกแบบเว็บไซต์
- Mobile App Design - ออกแบบแอปมือถือ
- Prototype - สร้างต้นแบบที่มี Interaction ได้
- Design System - จัดการระบบออกแบบองค์กร
- Collaboration - ทำงานเป็นทีมได้อย่างมีประสิทธิภาพ

---

## 2. Getting Started (เริ่มต้นใช้งาน)

### การสมัครและ Login

#### สมัครบัญชี
1. เข้าไปที่ figma.com
2. คลิก "Sign up" หรือ "Get started for free"
3. สมัครด้วย Email Address, Google Account หรือ Apple ID
4. ยืนยันอีเมล (กรณีสมัครด้วย Email)

#### แผนการใช้งาน
- **Starter Plan (ฟรี)** - เหมาะสำหรับนักเรียน นักศึกษา และผู้เริ่มต้น
  - 3 Figma files และ 3 FigJam files
  - Unlimited personal files
  - Unlimited cloud storage

### หน้า Dashboard

#### Recents
- ไฟล์ที่เปิดล่าสุด
- เข้าถึงงานที่กำลังทำได้รวดเร็ว

#### Drafts
- ไฟล์ร่างส่วนตัว
- ไฟล์ที่ยังไม่ได้จัดเก็บในโปรเจค

#### Projects
- โฟลเดอร์สำหรับจัดระเบียบไฟล์
- สามารถสร้างหลาย Project ได้
- แชร์ Project กับทีมงานได้

#### Community
- แหล่งรวม Template ฟรี
- ดู Design File จากผู้อื่น
- แชร์ผลงานของตัวเอง
- หา Inspiration และไอเดีย

### สร้างไฟล์ใหม่

#### New Design File
1. คลิก "New design file" หรือกด Ctrl/Cmd + N
2. ได้ Canvas ว่างเปล่าสำหรับออกแบบ
3. ตั้งชื่อไฟล์ที่มุมบนซ้าย

#### Frame/Artboard
- Frame = พื้นที่ทำงาน เหมือน Artboard ในโปรแกรมอื่น
- ใช้สำหรับกำหนดขนาดหน้าจอ (iPhone, iPad, Desktop)
- สามารถมีหลาย Frame ในไฟล์เดียวได้

#### Canvas Navigation
- **Zoom In/Out** - Ctrl/Cmd + / Ctrl/Cmd - หรือใช้ Mouse Wheel
- **Zoom to Fit** - Shift + 1
- **Pan** - Space + Drag หรือใช้ Hand Tool (H)

---

## 3. Basic Tools & Features (เครื่องมือและฟีเจอร์พื้นฐาน)

### a. Basic Tools

#### Move Tool (V)
- เลือกและย้ายวัตถุ
- ปรับขนาดโดยลาก Handle
- Rotate โดยลากนอก Bounding Box

**Shortcuts:**
- V - เปิด Move Tool
- Ctrl/Cmd + A - เลือกทั้งหมด
- Ctrl/Cmd + D - Duplicate
- Ctrl/Cmd + G - Group

#### Frame Tool (F)
- สร้างกรอบสำหรับออกแบบ
- มี Preset: Phone, Tablet, Desktop, Watch
- สามารถกำหนดขนาดเองได้

#### Shape Tools
- **Rectangle (R)** - สร้างสี่เหลี่ยม
- **Ellipse (O)** - สร้างวงรี/วงกลม
- **Polygon** - สร้างรูปหลายเหลี่ยม
- **Star** - สร้างรูปดาว
- **Line (L)** - สร้างเส้นตรง

#### Pen Tool (P)
- วาดรูปอิสระ Vector
- คลิกเพื่อสร้างจุด
- Drag เพื่อสร้างเส้นโค้ง

#### Text Tool (T)
- ใส่ข้อความ
- รองรับ Google Fonts และ Local Fonts
- ปรับ Font, Size, Color, Spacing ได้

### b. Layers

#### Layer Panel
- อยู่ด้านซ้ายของหน้าจอ
- แสดงโครงสร้างของงานทั้งหมด
- เรียงจากบนลงล่าง = หน้าไปหลัง

#### การเรียงลำดับ Layer
- **Ctrl/Cmd + ]** - Bring Forward
- **Ctrl/Cmd + [** - Send Backward
- **Ctrl/Cmd + Alt + ]** - Bring to Front
- **Ctrl/Cmd + Alt + [** - Send to Back

#### Group (Ctrl/Cmd + G)
- จัดกลุ่มวัตถุที่เกี่ยวข้องกัน
- ง่ายต่อการจัดการและย้าย
- สามารถ Collapse/Expand ได้

### c. Properties Panel

#### Size
- Width (W) - ความกว้าง
- Height (H) - ความสูง
- Shift + Drag - คงสัดส่วน

#### Position
- X - ตำแหน่งแนวนอน
- Y - ตำแหน่งแนวตั้ง

#### Fill
- Solid Color - สีทึบ
- Gradient - ไล่สี
- Image - รูปภาพ

#### Stroke
- เพิ่มขอบให้วัตถุ
- ปรับสี, ความหนา
- ตำแหน่ง: Inside, Center, Outside

#### Corner Radius
- ทำมุมให้โค้งมน
- ปรับแต่ละมุมแยกได้

### d. Auto Layout

Auto Layout ช่วยจัดวางองค์ประกอบอัตโนมัติและ Responsive

#### วิธีใช้
1. เลือกวัตถุ
2. กด Shift + A
3. ปรับ Padding, Spacing, Direction

#### คุณสมบัติ
- **Direction** - Horizontal/Vertical
- **Spacing** - ระยะห่างระหว่างวัตถุ
- **Padding** - ระยะห่างด้านใน
- **Alignment** - จัดตำแหน่ง

#### ตัวอย่างการใช้งาน
- ปุ่มที่ปรับขนาดตามข้อความ
- Navigation Bar
- Card Layout

### e. Collaborative

#### แชร์ไฟล์
1. คลิกปุ่ม Share
2. Copy link
3. ส่งลิงก์ให้เพื่อนร่วมงาน

#### สิทธิ์การเข้าถึง
- **Can View** - ดูอย่างเดียว
- **Can Edit** - แก้ไขได้

#### Real-time Collaboration
- เห็นเคอร์เซอร์ของเพื่อนร่วมงาน
- เห็นการเปลี่ยนแปลงทันที
- ไม่มีปัญหา Conflict

### f. Community and Inspiration

#### Figma Community
- แหล่งรวม Template ฟรี
- UI Kits, Wireframe Kits
- Plugins และ Icons

#### Resource แนะนำ
- Material Design - Design System จาก Google
- iOS Kit - Design System จาก Apple
- Dashboard Template
- Landing Page Templates

---

## 4. Design Fundamentals (หลักการออกแบบ)

### a. Spacing and Alignment

#### 8px Grid System
- มาตรฐานที่ใช้กันแพร่หลาย
- ขนาด, ระยะห่าง, Padding ใช้ 8, 16, 24, 32...
- ทำงานได้ดีกับ Retina Display

#### Alignment
- Left Align - ชิดซ้าย
- Center Align - กึ่งกลาง
- Right Align - ชิดขวา

### b. Typography

#### หลักการเลือกฟอนต์
- **Readability** - อ่านง่าย
- **Font Pairing** - ใช้ 2-3 ฟอนต์ที่เข้ากัน
- **Hierarchy** - ขนาดต่างกันเพื่อแยกความสำคัญ

#### การตั้งค่า
- Font Family: Kanit, Roboto, Open Sans
- Font Size: H1 (48-64px), Body (16-18px)
- Line Height: 1.5x สำหรับ Body
- Letter Spacing

### c. Color Palette

#### การเลือกสี
- **Primary Color** - สีหลักของแบรนด์
- **Secondary Color** - สีรอง
- **Neutral Colors** - เทา, ดำ, ขาว
- **Accent Color** - สีเน้น

#### หลัก 60-30-10 Rule
- 60% สีหลัก
- 30% สีรอง
- 10% สีเน้น

### d. Grid and Layout System

#### Column Grid
**Desktop:** 12 Columns, Margin 80px, Gutter 24px
**Mobile:** 4 Columns, Margin 20px, Gutter 16px

#### Responsive Design
- Mobile First Approach
- Breakpoints: 375px, 768px, 1024px, 1440px

---

## 5. Components & Design System

### a. Create Component

#### Component คืออะไร
- วัตถุที่สร้างขึ้นเพื่อใช้ซ้ำได้
- แก้ Master แล้ว Instance เปลี่ยนตาม

#### การสร้าง
1. วาดวัตถุที่ต้องการ
2. คลิกขวา → Create Component (Ctrl/Cmd + Alt + K)
3. ตั้งชื่อ Component

### b. Design System

#### ประกอบด้วย
- Color Styles
- Text Styles  
- Components Library
- Grid System
- Guidelines

### c. Reusable Components

#### Button Component
- โครงสร้าง: Frame + Icon + Text
- Auto Layout: Padding 16/12px
- Variants: Primary, Secondary, Outline
- States: Default, Hover, Active, Disabled

#### Input Field Component
- โครงสร้าง: Label + Input Container + Helper Text
- States: Empty, Filled, Focused, Error, Disabled

#### Card Component
- โครงสร้าง: Image + Content + Footer
- Auto Layout Vertical
- Shadow Effect

### d. Plugins

#### การติดตั้ง
1. Plugins → Browse plugins
2. ค้นหา Plugin
3. Install

#### Plugin แนะนำ
- **Iconify** - ไอคอนหลักพันตัว
- **Unsplash** - รูปภาพฟรี
- **Content Reel** - สร้างข้อมูลตัวอย่าง
- **Autoflow** - สร้าง User Flow

---

## 6. Prototyping (การสร้างต้นแบบ)

### a. Link Frame

#### Prototype คืออะไร
- จำลองการทำงานของแอพ/เว็บ
- เชื่อมโยงหน้าต่างๆ เข้าด้วยกัน

#### การสร้าง
1. เปลี่ยนไป Prototype Mode (Shift + E)
2. Drag Connection จากวัตถุไปยัง Frame ปลายทาง
3. ตั้งค่า Interaction

### b. Interaction and Animation

#### Interaction Types
- On Click - คลิก
- On Hover - เลื่อนเมาส์ชี้
- On Drag - ลาก

#### Animation Types
- Instant - ไม่มี Animation
- Dissolve - ค่อยๆ ปรากฏ
- Slide In - เลื่อนเข้ามา
- Smart Animate - Animation อัจฉริยะ

#### Duration
- Fast: 200-300ms
- Normal: 300-500ms
- Slow: 500-800ms

### c. Preview and Testing

#### Present Mode
- กดปุ่ม Present หรือ Shift + Space
- ทดสอบ Interaction

#### Figma Mirror App
- ดาวน์โหลดบน iOS/Android
- ดู Prototype บนมือถือจริง
- Real-time Update

### d. Shared Prototype

#### การแชร์
1. กดปุ่ม Share
2. Copy link → Prototype view
3. ส่งลิงก์ให้ผู้ทดสอบ

#### การรับ Feedback
- ผู้ดูกด Comment
- พิมพ์ Feedback
- Reply หรือ Resolve

---

## สรุป

Figma เป็นเครื่องมือที่ทรงพลังสำหรับการออกแบบ UI/UX โดยมีจุดเด่น:

1. ใช้งานง่าย เหมาะกับผู้เริ่มต้น
2. ทำงานร่วมกันได้แบบ Real-time
3. มี Components และ Design System
4. สร้าง Prototype ได้ครบวงจร
5. Community ใหญ่ มี Resource เยอะ

### ขั้นตอนการเรียนรู้แนะนำ
1. ฝึกใช้ Basic Tools
2. ทำความเข้าใจ Design Fundamentals
3. สร้าง Components
4. ลองทำ Prototype จริง

---

**จัดทำโดย:** อาจารย์ชานนท์  
**สถาบัน:** วิทยาลัยอาชีวศึกษานครปฐม  
**วันที่:** มกราคม 2568
