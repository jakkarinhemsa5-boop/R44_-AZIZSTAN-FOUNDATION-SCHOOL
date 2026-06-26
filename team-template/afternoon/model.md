<!-- workshop-header -->
<img width="1347" height="127" alt="Coding Thailand 2026 header" src="https://github.com/user-attachments/assets/ba5cf267-f460-4fb0-b69b-c461ae061a3b" />

# Afternoon — Model

- **Input ที่ใช้:** ___รูปภาพ________
- **Classes:** ______2 class_________
- **จำนวนตัวอย่าง/class:** _____44__________
- **วิธีเชื่อมเข้า Edge Impulse:** [/] กล้อง/ไมค์ (`edge-impulse-linux`)  [ ] Modulino (`data-forwarder`)

## V1
- Accuracy (ใน Studio): __57.69__
- F1 score ราย class (class : F1): _____class a : 0.73 __class b : 0.94________
- class ที่ F1 ต่ำสุด: ______class A_________
- รูป Confusion Matrix: ![cm-v1](../assets/cm-v1.png)
- อ่านแล้วเห็นอะไร (class ไหนสับสนกับ class ไหน): class 1 และ class 2 สามารีถแยกแยะได้อย่างชัดเจน

## V2 (ถ้าทัน)
- แก้อะไรจาก V1: _______________
- Accuracy V2: ____  | ดีขึ้น/แย่ลงตรงไหน: _______________

## รันบนบอร์ด
- [/] deploy target = **Arduino UNO Q** → Build → import ใน App Lab → Run
- [/] ป้อน input จริงแล้ว prediction เปลี่ยนตาม
- คลิป/รูปตอนรัน: ![run](../assets/run.jpg)

## (ต่อยอด) Output logic
- threshold ที่ใช้: confidence ≥ __0.5__
- map class → output: _______________ (เช่น "เตือน" → Buzzer + Pixels แดง)
