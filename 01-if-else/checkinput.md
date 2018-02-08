# 1.​โจทย์ ปัญหา 1 ข้อ ที่ต้องการใช้ if-else, Relation Operators และ/หรือ Logical Operators ในการแก้ปัญหา

จงเขียนโปรแกรมเพื่อนตรวจสอบว่า input ที่รับเข้ามามีค่าเป็นตัวพิมพ์ใหญ่ ตัวพิมพ์เล็ก ตัวเลข หรือว่าเป็นสัญลักษณ์พิเศษ
โดยให้เช็คแค่ตัวอักษรตัวแรกเท่านั้น โดยที่แสดงข้อความ "THIS PROGRAM CHECK ONLY FIRST CHARACTER!!!"

#include​<stdio.h>

int​ ​main​()

## {

​char​ c;

​ printf​("​THIS PROGRAM CHECK ONLY FIRST CHARACTER!!​\n​");

​printf​("​Enter a character : ​");

​scanf​("​%c​",&c);

​ if​ (c >= ​'A'​ && c <= ​'Z'​)

​ printf​("​It is a upper case alphabet​");

​ else if​ (c >= ​'a'​ && c <= ​'z'​)

​printf​("​It is a lower case alphabet​");

​ else if​ (c >=​ '0' ​&& c <= ​'9'​)

​ printf​("​It is a digit​");

​else

​printf​("​It is a special character​");

​ return​ 0 ​;

## }

#3. Test Case ที่จะใช้ทดสอบชุดคำสั่งดังกล่าว พร้อมผลลัพธ์ของชุดคำสั่งสำหรับแต่ละ Test Case


# Case 1

# THIS PROGRAM CHECK ONLY FIRST CHARACTER!!

# Enter a character : a

# It is a lower case alphabet

# Case 2

# THIS PROGRAM CHECK ONLY FIRST CHARACTER!!

# Enter a character : 5

# It is a digit

