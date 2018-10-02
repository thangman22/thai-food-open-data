# Thai food Open data
รายชื่อ อาหารและขนมไทย ใน format json

## ทำไมต้องทำ
อาหารไทยมีอยู่เยอะมากๆ แต่เราไม่เคยมีรายชื่อ อาหารไทย หรือ ข้อมูลอาหารไทยที่สามารถเอาไปใช้งานได้เลย ก็เลยคิดว่าจะทำข้อมูลอาหารไทยใน Format ที่สามารถเอาไปใช้ในการวิเคราห์ข้อมูล หรือเขียนโปรแกรมได้ ก็เลยเปิด repo นี้มาให้ทุกคนมาช่วยกัน contribute

## Format ของ ข้อมูล

ตัวอย่างของ format

```json
{
  "name":  "หมูทอดกระเทียม",
  "eng_name": "pork garlic stir fried",
  "rice": "possible",
  "egg": "possible",
  "meat": ["pork"],
  "spicy": false,
  "seafood": false,
  "green_level": "none",
  "contain_nut": "possible",
  "contain_milk": "none",
  "avg_calories": 200,
  "cuisine": "thai"
}
```
| Name          |Type| Option        |
| ------------- |-------------|-------------|
| name          |Text| ชื่ออาหาร |
| eng_name  |Text     | ชื่อ อาหารภาษาอังกฤษ      |
| rice          |Text| มีข้าวมั้ย (possible, contain, not-contain)     |
| meat          |Array | มีเนื้อสัตว์อะไรบ้าง      |
| spicy         |Boolean| เผ็ดมั้ย      |
| seafood      |Boolean| มีอาหารทะเลมั้ย     |
| green_level      |Text| ระดับความรักสุขภาพ (vegetarian, vegan)     |
| contain_nut      |Text| มีถั่วมั้ย (possible,contain, not-contain)     |
| contain_milk      |Text| ใส่นมมั้ย (possible,contain, not-contain)     |
| avg_calories      |Number| ให้พลังงานประมาณเท่าไหร่     |
| cuisine      |Text| ประเภทอาหาร     |


## Contribute ยังไง
- ถ้าต้องการเพิ่มข้อมูล สามารถเปิด Pull Request เข้ามาได้เลย
- ถ้าต้องการเพิ่ม field ขอให้ไปเปิด เป็น issue และ เปิด Pull Request readme.md เข้ามา
- ถ้าไม่มั่นใจข้อมูลส่วนไหนให้ใส่ null เอาไว้
- พยายาม append list จาก ท้ายขึ้นมา

## License
- นี่คือ ข้อมูลสาธารณะใครอยากเอาไปใช้อะไรก็เอาไปใช้ได้เลย
