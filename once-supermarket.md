# ONCE Supermarket

          จงเขียนโปรแกรมการคำนวณเงินของแคชเชียร์ในห้างสรรพสินค้าแห่งหนึ่ง โดยให้ผู้ใช้พิมพ์ จำนวนของสินค้าเข้ามาแต่จะสามารถรับ
        ได้มากที่สุดแค่ 20 ชิ้น เท่านั้น และตามด้วยใส่ราคาของสินค้าแต่ละชิ้น โดยมีเงื่อนไขในการคิดเงิน คือ ถ้าสินค้าชิ้นไหนมีราคา
        ตั้งแต่ 100 ขึ้นไป ให้เสียค่า VAT 7% ของราคาชิ้นนั้น ถ้าสินค้าไหนราคาไม่ถึง 100 คือ ไม่เสียค่า VAT 

          หลังจากใส่ราคาเรียบร้อยแล้ว ให้โปรแกรมแสดงผลสรุปบิลว่ามีสินค้าแต่ละชิ้นราคาเท่าไหร่, ชิ้นไหนเสียค่า VAT เท่าไหร่, 
        ราคาทั้งหมดก่อนที่จะรวมกับค่า VAT, ค่า VAT ทั้งหมด และ ราคาสุกท้ายที่ต้องจ่าย(รวมค่า VAT แล้ว)


**หมายเหตุ** : ถ้าใส่จำนวนสินค้าเกิน 20 หรือน้อยกว่า 1 จะขึ้นขเอความว่า **Sorry, this register can handle from 1 to 20 items only.** และโปรแกรมจะบังคับให้ใส่จำนวนใหม่จนกว่าจะถูก 


**ตัวอย่าง Input/Output**

1. **Input**
```
----Welcome to ONCE Supermarket!!----
 I hope you will enjoy in our store :)

How many items are in your basket? -1
Sorry, this register can handle from 1 to 20 items only.
How many items are in your basket? 2
Enter price for item 1: 1
Enter price for item 2: 20

```
**Output**
```
      Price           VAT         Item Total
   ----------     ----------      ----------
         1.00           0.00            1.00
        20.00           0.00           20.00
   ----------     ----------      ----------
        21.00           0.00           21.00

Thank you for shopping at ONCE Supermarket!

```

2. **Input**
```
----Welcome to ONCE Supermarket!!----
 I hope you will enjoy in our store :)

How many items are in your basket? 5
Enter price for item 1: 120
Enter price for item 2: 50
Enter price for item 3: 400
Enter price for item 4: 450
Enter price for item 5: 75
```
**Output**
```
      Price           VAT         Item Total
   ----------     ----------      ----------
       120.00           8.40          128.40
        50.00           0.00           50.00
       400.00          28.00          428.00
       450.00          31.50          481.50
        75.00           0.00           75.00
   ----------     ----------      ----------
      1095.00          67.90         1162.90

Thank you for shopping at ONCE Supermarket!
```
