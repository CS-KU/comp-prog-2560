# Daily Parking

ในทุกๆวันห้างจะทำการคิดค่าบริการสำหรับจอดรถในอาคารจอดรถโดยมีค่าบริการดังนี้ จอดรถต่ำกว่า2ชั่วค่าบริการ 10 บาทกรณีจอดมากกว่า 2 ชั่วโมงขึ้นไปคิดค่าบริการชั่วโมงละ 20 บาท

ให้เขียนโปรแกรมรับค่าจำนวนรถที่จอดจำนวนชั่วโมงและนาทีที่ใช้ในการจอดของรถแต่ละคันพร้อมคิดคำนวณเป็นจำนวนเงินที่ได้จากการเก็บค่าจอดรถและแสดงผลเป็น “Input error ” ในกรณีที่ใส่ข้อมูลผิด

# Input/output

Input
-   car (int)
-   hour (int)
-   min (int)

Output
-   จำนวนเงินในแต่ละวันกับผลรวมรายได้แบบสัปดาห์ตามที่ผู้ใช้ต้องการดู

# Test case
Test case 1

    Enter car parking: 3
    Enter number of hours are you parking: 2
    Enter number of minutes are you parking: 3
    Enter number of hours are you parking: 2
    Enter number of minutes are you parking: 5
    Enter number of hours are you parking: 4
    Enter number of minutes are you parking: 5
    Today we get 190 baht

Test case 2

    Enter car parking: 3
    Enter number of hours are you parking: -1
    Enter number of minutes are you parking: 2
    input errors
    Enter number of hours are you parking: 1
    Enter number of minutes are you parking: 2
    Enter number of hours are you parking: -1
    Enter number of minutes are you parking: -2
    input errors
    Today we get 10 baht
