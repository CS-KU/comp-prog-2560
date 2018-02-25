# เก็บค่า Array จนกว่าจะป้อน 0

เขียนโปรแกรมโดยรับค่าจนกว่าจะป้อนค่า 0

รับค่า Enter a number (0 - 100) :   

ให้นิสิตป้อนค่า 1 ถึง 100 ไปจนกว่าจะป้อนค่า 0 หากป้อนค่ามากกว่า 100 หรือป้อนค่าน้อยกว่า 0 จะพิมพ์คำว่า ERROR ออกมาแล้วให้ใส่ป้อนค่าใหม่ หากป้อนค่า 0 ให้แสดงค่าทั้งหมดที่ป้อนในรูปแบบของ Lists จากนั้นให้ในค่าที่ป้อนมาบวกกันทีละบรรทัดแล้วแสดงผลรวมทั้งหมดก่อนจบการทำงาน  

## Test case

ตัวอย่าง input/output 1
```
Enter a number (0 - 100) : 1
Enter a number (0 - 100) : 2
Enter a number (0 - 100) : 3  
Enter a number (0 - 100) : 4  
Enter a number (0 - 100) : 0
Array :  
[1, 2, 3, 4]  
1
3
6
10
Total is 10.  
```

ตัวอย่าง input/output 2
```
Enter a number (0 - 100) : 1000  
ERROR
Enter a number (0 - 100) : 100
Enter a number (0 - 100) : 99  
Enter a number (0 - 100) : 98  
Enter a number (0 - 100) : 0
Array :  
[100, 99, 98]  
100
199
297
Total is 297.
```

ตัวอย่าง input/output 3
```
Enter a number (0 - 100) : 1000  
ERROR
Enter a number (0 - 100) : 2000
ERROR
Enter a number (0 - 100) : 3000
ERROR
Enter a number (0 - 100) : -6000
ERROR
Enter a number (0 - 100) : 0
Array :  
[]  
Total is 0.
```
