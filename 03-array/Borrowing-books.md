# Borrowing books
หอสมุดของมหาวิทยาลัยแห่งหนึ่งต้องการเก็บข้อมูลการยืมหนังสือในแต่ละวัน โดยต้องการแบ่งกลุ่มผู้ยืมหนังสือเป็น 3 กลุ่มคือ กลุ่มนิสิต/นักศึกษา กลุ่มบุคลากรในมหาวิทยาลัย และกลุ่มบุคคลทั่วไป 

จงเขียนโปรแกรมเพื่อรับข้อมูลจำนวนหนังสือที่ยืมและกลุ่มที่ผู้ยืมถูกจัดไว้ จากนั้นแสดงผลออกมาเป็นจำนวนคนที่ยืมหนังสือและจำนวนหนังสือที่ถูกยืมของแต่ละกลุ่ม ซึ่งกำหนดจำนวนคนในแต่ละกลุ่มให้เก็บข้อมูลได้สูงสุดเพียง 100 คน
### Input
กำหนดให้รับจำนวนหนังสือที่จะยืมและอักษรย่อของกลุ่มซึ่งจะคั่นด้วย ‘/’ ทีละบรรทัด จะหยุดการรับข้อมูลก็ต่อเมื่อใส่จำนวนเต็มที่มีค่าน้อยกว่าหรือเท่ากับ 0 หรือเป็นข้อมูลที่ไม่ใช่จำนวนเต็มในส่วนของจำนวนหนังสือ
ซึ่งการรับข้อมูลโดยตัวอักษรย่อนั้นได้แก่ s คือกลุ่มนิสิต/นักศึกษา, p คือกลุ่มบุคลากร และ g คือกลุ่มบุคคลทั่วไป
### Output
แสดงจำนวนคนที่ยืมหนังสือและจำนวนหนังสือที่ยืมในกลุ่มนิสิต/นักศึกษา กลุ่มบุคลากร และกลุ่มบุคคลทั่วไปตามลำดับ

*ถ้าตัวอักษรย่อไม่ตรงกับที่กำหนดเอาไว้จะไม่นับจำนวนหนังสือแต่ยังรับข้อมูลต่อได้*
### ตัวอย่าง Input-Output
```Enter incumbent/number of book(s) : 1/s
Enter incumbent/number of book(s) : 1/p
Enter incumbent/number of book(s) : 1/g
Enter incumbent/number of book(s) : 0
>>The number of students borrowing books is 1.
>>The total number of books borrowed by the student is 1.
>>The number of personnels borrowing books is 1.
>>The total number of books borrowed by the personnel is 1.
>>The number of general publics borrowing books is 1.
>>The total number of books borrowed by the general public is 1.
```
```Enter incumbent/number of book(s) : s
>>The number of students borrowing books is 0.
>>The total number of books borrowed by the student is 0.
>>The number of personnels borrowing books is 0.
>>The total number of books borrowed by the personnel is 0.
>>The number of general publics borrowing books is 0.
>>The total number of books borrowed by the general public is 0.
```

