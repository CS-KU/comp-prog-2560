#{C}ตั้งค่าตัวให้นักฟุตบอลไทยไปบอลโลก!!!
ให้นิสิตเขียนโปรแกรมตั้งค่าตัวให้นักฟุตบอล โดยปกติแล้วนัก
ฟุตบอลจะมีคนลงสนามอยู่ 11 คน แต่ละคนจะมีเบอร์เสื้อในโปรแกรมนี้ให้ใช้เบอร์ {1-11} แทนเบอร์เสื้อของนักฟุตบอล 
Input: รับค่าตัวนักฟุตบอลในหน่วยล้าน เช่น 20 ล้าน เป็นต้น
และอยู่ในช่วง 20 – 200 ล้านบาท โดยนักฟุตบอลที่มีราคาค่าตัวตั้งแต่ 
20 - 60 ล้านบาท จะไม่บวกภาษีเพิ่ม
61 - 100 ล้านบาท จะบวกภาษีเพิ่ม 5%
101 - 140 ล้านบาท จะบวกภาษีเพิ่ม 9%
141 - 180 ล้านบาท จะบวกภาษีเพิ่ม 13%
181 - 200 ล้านบาท จะบวกภาษีเพิ่ม 15%
Output1: พิมพ์ค่าตัวของนักฟุตบอลแต่ละคนที่บวกภาษีเพิ่มแล้ว
Output2: พิมพ์ภาษีที่บวกเพิ่มของนักฟุตบอลทั้ง 11 คน
Output3: พิมพ์ค่าตัวของนักฟุตบอลที่บวกภาษีเพิ่มแล้วทั้ง 11 คน

```
Enter value of footballer number {1}: 100
Enter value of footballer number {2}: 110
Enter value of footballer number {3}: 120
Enter value of footballer number {4}: 130
Enter value of footballer number {5}: 140
Enter value of footballer number {6}: 150
Enter value of footballer number {7}: 160
Enter value of footballer number {8}: 170
Enter value of footballer number {9}: 180
Enter value of footballer number {10}: 190
Enter value of footballer number {11}: 200


Value of footballer + tax is:

>>>number {1} = 105.00 million baht.
>>>number {2} = 119.90 million baht.
>>>number {3} = 130.80 million baht.
>>>number {4} = 141.70 million baht.
>>>number {5} = 152.60 million baht.
>>>number {6} = 169.50 million baht.
>>>number {7} = 180.80 million baht.
>>>number {8} = 192.10 million baht.
>>>number {9} = 203.40 million baht.
>>>number {10} = 218.50 million baht.
>>>number {11} = 230.00 million baht.

All taxes must be paid 194.30 million baht.

All value of footballer + tax is: 1844.30 million baht.
```
Test cases:
ถ้าใส่ค่าที่เป็น float หรือใส่ตัวอักษรมาจะเป็น  Infinity loop
```
Enter value of footballer number {1}: 123.00
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
Enter value of footballer number {2}: Invalid
```
```
Enter value of footballer number {1}: j
Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
Enter value of footballer number {1}: Invalid
```
ถ้าใส่ค่านอกเหนือจากที่กำหนดจะ printf Invalid และทำการรับค่าในตำแหน่งนั้นใหม่
```
Enter value of footballer number {1}: -1
Invalid
Enter value of footballer number {1}: -16232
Invalid
Enter value of footballer number {1}: 665153213
Invalid
Enter value of footballer number {1}: 12
Invalid
Enter value of footballer number {1}: 20
Enter value of footballer number {2}:
```
นายณัฐพงษ์ รุ่งเรือง รหัสนิสิต: 6010405220