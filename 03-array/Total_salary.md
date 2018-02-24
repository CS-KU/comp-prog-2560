# *ให้คำนวณเงินเดือนพนักงาน*
ในบริษัทแห่งหนึ่ง มีพนักงานจำนวน 5 คน ให้ทำการรับข้อมูล รหัสพนักงาน  เงินเดือน และโบนัสแต่ละคน แล้วนำมาคำนวณ รายได้แต่ละคน พร้อมทั้งนำเงินได้ทั้งหมดไปหักภาษี ดังนี้ 
 - ถ้าเงินรวมทั้งหมด มีค่าตั้งแต่  0-2000 บาท / เดือน  ไม่ต้องหักภาษี ณ ที่จ่าย
 - ถ้าเงินรวมทั้งหมด มีค่าตั้งแต่  2001-10000 บาท / เดือน  หักภาษี ณ ที่จ่าย 5%
 - ถ้าเงินรวมทั้งหมด มีค่าตั้งแต่ 10001-20000 บาท / เดือน  หักภาษี ณ ที่จ่าย 7%
 - ถ้าเงินรวมทั้งหมด มีค่าตั้งแต่  20001-50000 บาท / เดือน  หักภาษี ณ ที่จ่าย 8%
 - ถ้าเงินรวมทั้งหมด มีค่าตั้งแต่  50001 ขึ้นไป / เดือน  หักภาษี ณ ที่จ่าย 10%

ให้เขียนโปรแกรมเพื่อทำการคำนวณค่า พนักงานแต่ละคน จะได้รับเงินทั้งหมด หลังหักภาษี ณ ที่จ่าย เป็นเงินเท่าไร และบริษัทจะต้องจ่ายเงินให้แก่พนักงานทั้งบริษัทเป็นเงินเท่าไร

## *Input/output*
- Input  
    - ให้ employee_ID[5]; ใส่รหัสพนักงงานบริษัท
    - ให้ salary[5] เป็นเงินเดือน
    - ให้ bonus[5] เป็นโบนัส
- output  
    - ให้ y[] เป็นเงินเดือนที่ต้องจ่ายให้พนักงาน
    - ให้ Total[] เป็นเงินเดือนที่ต้องจ่ายท้ังหมด
---
*Testcase 1*
```
***1.Enter Data***
Enter employee ID[1]: 1001
Enter salary[1]: 2000
Enter bonus[1]: 300
Enter employee ID[2]: 1002
Enter salary[2]: 4000
Enter bonus[2]: 400
Enter employee ID[3]: 1003
Enter salary[3]: 5000
Enter bonus[3]: 600
Enter employee ID[4]: 1004
Enter salary[4]: 6000
Enter bonus[4]: 500
Enter employee ID[5]: 1005
Enter salary[5]: 7000
Enter bonus[5]: 700

***2. Display ****

Total salary[1]: 2200.00
Total salary[2]: 4200.00
Total salary[3]: 5350.00
Total salary[4]: 6200.00
Total salary[5]: 7350.00

***Total balance = 26500.00***
```
---
*Testcase 2*
```
***1.Enter Data:***
Enter employee ID[1]: 1
Enter salary[1]: 44350
Enter bonus[1]: 3000
Enter employee ID[2]: 2
Enter salary[2]: 97000
Enter bonus[2]: 6000
Enter employee ID[3]: 3
Enter salary[3]: 33000
Enter bonus[3]: 4000
Enter employee ID[4]: 4
Enter salary[4]: 25000
Enter bonus[4]: 2000
Enter employee ID[5]: 5
Enter salary[5]: 11000
Enter bonus[5]: 1000

***2. Display ****

Total salary[1]: 43802.00
Total salary[2]: 93300.00
Total salary[3]: 34360.00
Total salary[4]: 25000.00
Total salary[5]: 11230.00

***Total balance = 226350.00***
```