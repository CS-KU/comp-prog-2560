# โปรแกรมคำนวณหาพิกัดและระยะห่างระหว่างจุด A และจุด B

จงเขียนโปรแกรมที่รับค่า x และค่า y ของจุด A และจุด B และทำการบอกทิศทางของจุดทั้งสองจากจุดศูณย์กลาง (0,0) โดยจะมีทั้งหมด 8 ทิศทางดังนี้ 

(North, South, East, West, North-east, North-west, South-east, South-west)

และเมื่อทำการบอกทิศทางของทั้งสองจุดเรียบร้อยแล้วให้ทำการคำณวนระยะห่างของทั้งสองจุด โดยจะสามารถคำณวนระยะห่างได้จากสูตรสามเหลี่ยมมุมฉาก

**หมายเหตุ** หากจุด A หรือ B รับค่าเป็น (0,0) แม้แต่จุดเดียวให้แสดงผลลัพธ์เป็น ERROR ทั้งหมดทันที

### **ตัวอย่าง** **Input/Output**

```
Point A
Enter X : 0
Enter Y : 0
Point A place : ERROR
Point B
Enter X : 1
Enter Y : 6
Point B place : ERORR
Point distance : ERORR
```
```
Point A
Enter X : -3
Enter Y : 2
Point A place : North-west
Point B
Enter X : 1
Enter Y : -1
Point B place : South-east
Point distance : 5
```
```
Point A
Enter X : 0
Enter Y : 0
Point A place : ERROR
Point B
Enter X : 0
Enter Y : 0
Point B place : ERORR
Point distance : ERORR
```


