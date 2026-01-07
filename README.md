# Avatar-Zeless-ID
# 🎮 Zenless Zone Zero - Avatar ID Mapping

ไฟล์นี้รวบรวมรายการข้อมูล **Avatar ID** และ **ชื่อตัวละคร** ภายในเกม Zenless Zone Zero (ZZZ) เพื่อใช้สำหรับการอ้างอิงในการพัฒนา Mod, จัดทำฐานข้อมูล หรือการดึงข้อมูล (Data Scraping)

---

## 📄 ข้อมูลโครงสร้าง (Data Structure)

ข้อมูลชุดนี้จัดเก็บในรูปแบบ JSON ประกอบด้วย Object หลักคือ `AvatarNames` ที่ใช้ ID เป็นตัวเลข 4 หลักจับคู่กับชื่อทางการของตัวละคร

## 📋 รายการตัวละคร (Character List)

| ID | ชื่อตัวละคร (Character Name) |
| :--- | :--- |
| **1011** | Anby Demara |
| **1021** | Nekomiya Mana |
| **1031** | Nicole Demara |
| **1041** | Soldier 11 |
| **1051** | Yidhari Murphy |
| **1061** | Corin Wicker |
| **1071** | Caesar King |
| **1081** | Billy Kid |
| **1091** | Hoshimi Miyabi |
| **1101** | Koleda Belobog |
| **1111** | Anton Ivanov |
| **1121** | Ben Bigger |
| **1131** | Soukaku |
| **1141** | Von Lycaon |
| **1151** | Luciana de Montefio |
| **1161** | Lighter |
| **1171** | Burnice White |
| **1181** | Grace Howard |
| **1191** | Ellen Joe |
| **1201** | Asaba Harumasa |
| **1211** | Alexandrina Sebastiane |
| **1221** | Tsukishiro Yanagi |
| **1241** | Zhu Yuan |
| **1251** | Qingyi |
| **1261** | Jane Doe |
| **1271** | Seth Lowell |
| **1281** | Piper Wheel |
| **1291** | Hugo Vlad |
| **1301** | Orphin Magnusson & Magus |
| **1311** | Astra Yao |
| **1321** | Evelyn Chevalier |
| **1331** | Vivian Banshee |
| **1341** | Xiao Zhao |
| **1351** | Pilchra Fellini |
| **1361** | Trigger |
| **1371** | Yixuan |
| **1381** | Soldier 0 - Anby |
| **1391** | Ju Fufu |
| **1401** | Alice Thymefield |
| **1411** | Ukinami Yuzuha |
| **1421** | Pan Yinhu |
| **1431** | Ye Shunguang |
| **1441** | Komano Manato |
| **1451** | Lucia Elowen |
| **1461** | Seed |
| **1471** | Banyue |
| **1481** | Dialyn |
| **1491** | Sunna |
| **1501** | Aria |
| **2071** | Idk |

---

## 🛠️ การนำไปใช้งาน (Usage)

คุณสามารถนำข้อมูล JSON ไปใช้ในโปรเจกต์ของคุณได้ดังนี้:

### ตัวอย่างการเข้าถึงข้อมูล (JavaScript)
```javascript
const data = {
  "AvatarNames": {
    "1011": "Anby Demara",
    "1191": "Ellen Joe"
    // ...
  }
};

const getCharacter = (id) => data.AvatarNames[id] || "ไม่พบข้อมูล";
console.log(getCharacter("1011")); // Anby Demara
