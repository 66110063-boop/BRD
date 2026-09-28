# 🎨 UI/UX Design System & Principles Repository
> **คลังข้อกำหนดมาตรฐานและหลักการออกแบบส่วนติดต่อผู้ใช้ (Design Guidelines & Design Tokens)**  
> รวบรวมแนวคิดการออกแบบ **Hallmark Anti-AI-Slop Guidelines (v1.1.0)** และมาตรฐาน **KTB Theme Design System**

---

## 📁 โครงสร้างไฟล์ใน Repository (Repository Structure)

```text
├── DESIGN_GUIDELINES.md   # คู่มือและหลักการออกแบบฉบับสมบูรณ์ (สเปก, โทเค็น, UX/UI, สูตร Prompt AI)
├── tokens.css             # ไฟล์ CSS Design Tokens (สี, ฟอนต์, สัดส่วน, Radius, กฎ Zero Box-shadow)
├── .gitignore             # Git ignore configuration
└── README.md              # เอกสารแนะนำภาพรวมของ Repository
```

---

## 🌟 จุดเด่นและแกนหลักในการออกแบบ (Key Architectural Principles)

### 1. Hallmark Anti-AI-Slop (v1.1.0)
* **Zero Box-Shadow:** กำจัดเงาฟุ้งแบบ generic ทิ้งทั้งหมด โดยใช้ Hairline Rule `1px solid #E3E7EA`
* **Flat Paneling & Chunking:** แบ่งสัดส่วนชัดเจนแบบ Workbench 7:5 หรือ Master-Detail 6:4
* **WCAG AA Compliance:** อัตราส่วนความเปรียบต่างสี (Contrast Ratio) ผ่านเกณฑ์ ≥ 4.5:1 ทุกจุด
* **Senior & Operator Ergonomics:** ออกแบบเพื่อการใช้งานจริง อ่านง่าย รวดเร็ว สระไม่ลอย

### 2. KTB Theme Design Standards (21 กันยายน 2569)
* **Typography:** ใช้แบบอักษร `Anuphan` เฉพาะ 3 น้ำหนัก (`400 Regular`, `500 Medium`, `600 SemiBold`) **ห้ามใช้ Bold 700**
* **Frame Constraints:** ขนาดตายตัว **`Width: 1280px`** และ **`Height: 860px`** ควบคุมด้วย `overflow: hidden;` ห้ามเกิด Scrollbar หน้าต่างที่ 100% Zoom
* **Color Palette:**
  * Brand Identity: `--ktb-brand: #00A5E5`
  * Action & Interactive: `--ktb-action: #007AAE` (Contrast 4.78:1)
  * Active Tint: `--ktb-action-tint: #E6F6FD`
  * Dark Headers: `--primary-dark: #1E293B`
  * Borders & Dividers: `--line-200: #E3E7EA`
  * Surfaces: Canvas `--canvas: #F7F9FA` / Card `--paper: #FFFFFF`
  * Status Semantic: Success `#14865A`, Warning `#946011`, Danger `#B3261E`

---

## 📖 เอกสารอ่านเพิ่มเติม
* ศึกษารายละเอียดสเปกการออกแบบทั้งหมด สัดส่วน Layout และโครงสร้างคำสั่งสั่ง AI ได้ที่ **[DESIGN_GUIDELINES.md](DESIGN_GUIDELINES.md)**
* เรียกใช้ CSS Variables ทั้งหมดได้จากไฟล์ **[tokens.css](tokens.css)**
