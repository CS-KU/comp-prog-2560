# Palindrome

เลขพาลินโดรม คือชุดของตัวเลขที่เรียงต่อกัน ซึ่งมีการเรียงที่เท่ากันทั้งจากหลังมาหน้าและหน้าไปหลัง เช่น พาลินโดรม 3 หลัก: 303, พาลินโดรม 4 หลัก: 5115, พาลินโดรม 5 หลัก: 78087, พาลินโดรม 6 หลัก: 296692, พาลินโดรม 7 หลัก: 4961694

จงเขียนโปรแกรมรับค่าเลข 1 ชุด 7 หลัก แล้วตรวจสอบว่า เลขชุดนี้เป็น Palindrome หรือไม่

### Input
1.  รับค่าเลขทีละตัว ทั้งหมด 7 ตัว โดยแสดงข้อความว่า Enter number:

### Output
1.  ถ้าเลขชุดนี้เป็นพาลินโดรม ข้อความที่จะแสดงออกมาจะแสดงเลขที่รับค่าออกมาก่อน แล้วบอกว่าเป็นพาลินโดรม เช่น 1564651 is Palindrome.
2.  ถ้าเลขชุดนี้ไม่เป็นพาลินโดรม ข้อความที่แสดงออกมาจะแสดง เลขที่รับค่าออกมาก่อน แล้วบอกว่าไม่เป็นพาลินโดรม เช่น 8306302 is NOT Palindrome.

ถ้าข้อมูลที่รับมาไม่ถูกต้อง คือ เลขที่รับมามากกว่า 1 ตัว หรือเลขที่รับมาติดลบ ให้พิมพ์ว่า Invalid input!

**ตัวอย่าง Input/Output1**
#### input:
         Enter number: 2
         Enter number: 7
         Enter number: 8
         Enter number: 1
         Enter number: 8
         Enter number: 7
         Enter number: 2
#### output:
         2781872 is Palindrome.

**ตัวอย่าง Input/Output2**
#### input:
         Enter number: 9
         Enter number: 6
         Enter number: 3
         Enter number: 2
         Enter number: 3
         Enter number: 8
         Enter number: 6
#### output:
         9632386 is NOT Palindrome.

**ตัวอย่าง Input/Output3**
#### input:
         Enter number: 4
         Enter number: 65
         Enter number: 1
         Enter number: 0
         Enter number: 1
         Enter number: 56
         Enter number: 4
#### output:
         Invalid input!
