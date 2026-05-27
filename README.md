# profile
อ้อง่ายนิดเดียวคำตอบคือ 67
# ยินดีต้อนรับสู่ GitHub ของฉัน 👋

## 👤 ข้อมูลส่วนตัว (About Me)
* **ชื่อ-นามสกุล:** [ใส่ชื่อ-นามสกุลของคุณที่นี่]
* **การศึกษา:** นักศึกษา วิทยาลัยพณิชยการบางนา
* **สาขาวิชา:** เทคโนโลยีสารสนเทศ (Information Technology)

<div align="center">
    <img src=:https://rms.bncc.ac.th/files/importpicstd/01/69319010016.jpg" alt="My Profile Picture" width="200" style="border-radius: 50%;">
</div>

---

## 🎯 จุดประสงค์ในการเข้าศึกษาต่อ
เหตุผลและเป้าหมายที่ฉันเลือกเข้าศึกษาต่อที่ **วิทยาลัยพณิชยการบางนา สาขาเทคโนโลยีสารสนเทศ** มีดังนี้:

* **พัฒนาทักษะด้าน IT:** เพื่อเรียนรู้ระบบสารสนเทศและการเขียนโปรแกรมอย่างเป็นมืออาชีพ
* **ต่อยอดสู่อนาคต:** นำความรู้ไปประยุกต์ใช้ในการทำงานจริงในยุคดิจิทัล และสร้างสรรค์เทคโนโลยีที่เป็นประโยชน์
* **ความหลงใหลส่วนตัว:** มีความสนใจในระบบการทำงานเบื้องหลัง (Backend) และต้องการพัฒนาซอฟต์แวร์ที่มีประสิทธิภาพ

---

## 💻 รายวิชาที่กำลังศึกษา: Backend Development
ในรายวิชานี้เน้นการเรียนรู้ระบบการทำงานหลังบ้าน การจัดการเซิร์ฟเวอร์ และการเชื่อมต่อฐานข้อมูล

### 📚 หัวข้อหลักที่ศึกษา (Main Topics)
1.  **Introduction to Node.js & Runtime Environment**
    * ทำความเข้าใจเกี่ยวกับ Event-Driven และ Non-blocking I/O
2.  **RESTful API Development**
    * การสร้าง API เพื่อให้ฝั่ง Frontend สามารถเรียกใช้งานข้อมูลได้
3.  **Database Management**
    * การเชื่อมต่อและจัดการฐานข้อมูล (เช่น MongoDB, MySQL)

### 🔍 หัวข้อย่อยที่น่าสนใจ (Sub-topics)
* การใช้งาน **Express.js** Framework
* การจัดการ HTTP Methods (`GET`, `POST`, `PUT`, `DELETE`)
* การทำ Authentication & Authorization (เช่น JWT)
* การทดสอบ API ด้วยโปรแกรม **Postman**

---

## 🚀 ตัวอย่างการเขียน Code ด้วย Node.js
นี่คือตัวอย่างการสร้าง HTTP Server อย่างง่ายด้วย Node.js และ Express.js เพื่อแสดงข้อความ "Hello World" และการสร้าง API ส่งข้อมูล JSON

```javascript
// 1. นำเข้า Express Module
const express = require('express');
const app = express();
const PORT = 3000;

// รองรับการอ่านข้อมูลแบบ JSON
app.use(express.json());

// 2. สร้าง Route สำหรับหน้าแรก (Homepage)
app.get('/', (req, res) => {
    res.send('ยินดีต้อนรับเข้าสู่ Backend Server ของฉัน!');
});

// 3. สร้าง API Route สำหรับดึงข้อมูลตัวอย่าง (GET Method)
app.get('/api/user', (req, res) => {
    res.json({
        id: 1,
        name: "[ชื่อของคุณ]",
        major: "Information Technology",
        college: "Bangna College of Commerce"
    });
});

// 4. สั่งให้ Server ทำงานที่ Port ที่กำหนด
app.listen(PORT, () => {
    console.log(`Server is running at http://localhost:${PORT}`);
});
