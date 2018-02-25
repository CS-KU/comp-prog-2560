# OX GAMES

เขียนโปรแกรมเล่นเกม OX ขนาด 3x3 และแสดงผลเป็นผลของการเล่น โดยเลขช่องเป็นดังนี้


| 1 | 2 | 3 |
|---|---|---|
| 4 | 5 | 6 |
| 7 | 8 | 9 |


ข้อมูลนำเข้า
- แสดงข้อความ “Enter your position and ox: ” นำเข้าเป็นช่องที่ต้องการลงและตัวอักษร O หรือ X ของผู้
เล่นที่ต้องการลงในช่องนั้น และคั่นกลางด้วย “-”

ข้อมูลนำออก
- รูปแบบของ ox ที่ถูกวางลงในช่อง
เกิดข้อผิดพลาด
- ช่องที่ต้องการลงไม่ตรงตามเลขดังภาพ แสดงผล “Sorry, you can't play this game (your position is
wrong.) ” และหยุดรับข้อมูลนำข้าและแสดงค่าเริ่มต้นหมดทุกช่องออกมา
- ตัวอักษรที่นำเข้าไม่ใช่ O หรือ X แสดงผล “Sorry, you can't play this game (your ox is wrong.)” และ
หยุดรับข้อมูลนำเข้าและแสดงค่าเริ่มต้นหมดทุกช่องออกมา
- ถ้าเกิดผิดทั้งสองอย่าง แสดงผล “Sorry, you can't play this game (your position is wrong.) ” และหยุดัรบข้อมูลนำเข้าและแสดงค่าเริ่มต้นหมดทุกช่องออกมา

** โปรแกรมนี้สามารถรับค่าช่องซ้ าได้แต่ใส่ได้ทั้งหมดแค่ 9 ครั้งเท่านั้น ส่วนช่องที่ไม่ได้เลือกใส่ค่าเริ่มต้น

** รับข้อมูลนำเข้าตัวอักษรได้ทั้งพิมพ์เล็กและพิมพ์ใหญ่

** ค่าเริ่มต้น คือ -

## ตัวอย่าง Input/Output

ตัวอย่างที่ 1

    --------------------------------
    ------------OX GAMES------------
    --------------------------------
    Enter your position and ox: 1-o
    Enter your position and ox: 2-o
    Enter your position and ox: 3-o
    Enter your position and ox: 4-o
    Enter your position and ox: 5-o
    Enter your position and ox: 6-o
    Enter your position and ox: 7-o
    Enter your position and ox: 8-o
    Enter your position and ox: 9-o
    --------------------------------
                |O|O|O|
                |O|O|O|
                |O|O|O|
    --------------------------------
ตัวอย่างที่ 2

    --------------------------------
    ------------OX GAMES------------
    --------------------------------
    Enter your position and ox: 1-x
    Enter your position and ox: 3-x
    Enter your position and ox: 4-x
    Enter your position and ox: 5-o
    Enter your position and ox: 6-x
    Enter your position and ox: 7-o
    Enter your position and ox: 7-x
    Enter your position and ox: 8-x
    --------------------------------
                |X|O|X|
                |X|O|X|
                |X|X|-|
    --------------------------------