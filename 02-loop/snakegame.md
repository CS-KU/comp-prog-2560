# เกมบันไดงู
ให้เขียนโปรแกรมสำหรับการเล่นเกมบันไดงู โดยแสดงผลผู้ชนะในเกม เมื่อเล่นเสร็จจะแสดงผู้ที่ชนะและผลของคะแนนที่ได้ โดยค่าที่
นำเข้าเป็นจำนวนเต็มทั้งหมด

-   คะแนนนั้นคิดได้จากถ้าผู้ที่ชนะจะได้คะแนน 1 คะแนน ส่วนผู้แพ้ได้ 0 คะแนน

สัญลักษณ์ในภาพด้านล่างคือ
1. บันได: ถ้าเดินตกตรงนั้นจะเดินขึ้นไปยังช่องที่บันไดพาดไว้
2. งู:  ถ้าเกิดเดินไปยังช่องนั้นแล้วจะเดินย้อนกลับมาที่ช่องที่หัวงูชี้ไป
3. X: เดินเพิ่มคูณจากจำนวนช่อง
4. ^(หมายเลข): เดินขึ้นไปที่ช่องหมายเลขนั้น


ถ้ารับจำนวนครั้งมีข้อผิดพลาดจะแสดงผล เป็น “Sorry, You can't play this games.” แล้วหยุดการทำงาน แต่สำหรับ
ค่าของการทอยลูกเต๋ามีข้อผิดพลาดจะแสดงผล เป็น “Sorry, You can't play this games.” แต่จะทำการเล่นรอบต่อไปและคิด
คะแนนปกติ

ข้อมูลนำเข้า
1. จำนวนครั้งที่ต้องการเล่น แสดงข้อความเป็น “Enter amount of round play: ”
2. รับค่าของลูกเต๋าที่ทอยเรื่อยจนจบเกม แสดงข้อความเป็น “Enter Player1's value of dice: ” หรือ Enter
Player2's value of dice: ”

ข้อมูลนำออก
1. ผู้ที่ชนะในรอบนั้น “THE WINNER IN ROUND 2: ผู้ชนะ”
2. ผู้ที่ชนะที่คะแนนมากที่สุด

[![snake.png](http://upload.sodazaa.com/images/2018/02/24/snake.png)](http://upload.sodazaa.com/image/WfiFJ)

## ตัวอย่าง Input/Output

ตัวอย่างที่1

    -----------------------------------------
    Enter amount of round play: 2
    -----------------------------------------
    ---------------<<ROUND 1>>---------------
    Enter Player1's value of dice: 7
    Sorry, You can't play this games.
    -----------------------------------------
    ---------------<<ROUND 2>>---------------
    Enter Player1's value of dice: 5
    Totals1 : 19
    Totals2 : 0
    Enter Player2's value of dice: 6
    Totals1 : 19
    Totals2 : 18
    Enter Player1's value of dice: 5
    Totals1 : 38
    Totals2 : 18
    Enter Player2's value of dice: 6
    Totals1 : 38
    Totals2 : 36
    Enter Player1's value of dice: 5
    Totals1 : 57
        Totals2 : 36
    Enter Player2's value of dice: 6
    Totals1 : 57
    Totals2 : 54
    Enter Player1's value of dice: 5
    Totals1 : 62
    Totals2 : 54
    -----------------------------------------
    THE WINNER IN ROUND 2: Player1
    ---------------<<FINAL>>---------------
    --------THE WINNER : Player1--------
    Score: - Player1 = 1
    - Player2 = 0
    -----------------------------------------

ตัวอย่างที่2

    -----------------------------------------    
    Enter amount of round play: 0
    -----------------------------------------
    Sorry, You can't play this games.
    -----------------------------------------
