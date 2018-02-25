# Weekly Parking

ในทุกวันห้างจะทำการคิดค่าบริการสำหรับจอดรถในอาคารจอดรถโดยมีค่าบริการดังนี้ จอดรถต่ำกว่า 2 ชั่วค่าบริการ 10 บาทกรณีจอดมากกว่า 2 ชั่วโมงขึ้นไปคิดค่าบริการชั่วโมงละ 20 บาท

ให้เขียนโปรแกรมรับค่าจำนวนรถที่จอดจำนวนชั่วโมงและนาทีที่ใช้ในการจอดของรถแต่ละคันพร้อมคิดคำนวณเป็นจำนวนเงินที่ได้จากการเก็บค่าจอดรถและให้แสดงผลเป็นให้เลือกดูจำนวนเงินที่ได้จากการเก็บค่าจอดรถในแต่ละวันหรือผลรวมรายสัปดาห์และแสดงผลเป็น “Input error ” ในกรณีที่ใส่ข้อมูลผิด

(กำหนดให้ใช้Arrayในการเก็บข้อมูลค่าจอดแต่ละวัน)

# Input/output

Input
-   car (int)
-   hour (int)
-   min (int)

Output
-   จำนวนเงินในแต่ละวันกับผลรวมรายได้แบบสัปดาห์ตามที่ผู้ใช้ต้องการดู

# Test case
Test case 1

    Enter car parking: -1
    input error
    what do you want to show you cost: 1 = monday 2 = tuesday 3 = wenday 4 = thursday 5 = friday 6 = satday 7 = sunday 8 = allweek
    input errors

Test case 2

    Enter car parking: 1
    Enter number of hours are you parking: 2
    Enter number of minutes are you parking: 3
    Enter car parking: 2
    Enter number of hours are you parking: 3
    Enter number of minutes are you parking: 4
    Enter number of hours are you parking: 5
    Enter number of minutes are you parking: 3
    Enter car parking: 4
    Enter number of hours are you parking: 1
    Enter number of minutes are you parking: 2
    Enter number of hours are you parking: 1
    Enter number of minutes are you parking: 50
    Enter number of hours are you parking: 2
    Enter number of minutes are you parking: 4
    Enter number of hours are you parking: 5
    Enter number of minutes are you parking: 30
    Enter car parking: 1
    Enter number of hours are you parking: 4
    Enter number of minutes are you parking: 53
    Enter car parking: 2
    Enter number of hours are you parking: 3
    Enter number of minutes are you parking: 36
    Enter number of hours are you parking: 2
    Enter number of minutes are you parking: 45
    Enter car parking: 2
    Enter number of hours are you parking: 4
    Enter number of minutes are you parking: 50
    Enter number of hours are you parking: 3
    Enter number of minutes are you parking: 50
    Enter car parking: 1
    Enter number of hours are you parking: 2
    Enter number of minutes are you parking: 30
    what do you want to show you cost: 1 = monday 2 = tuesday 3 = wenday 4 = thursday 5 = friday 6 = satday 7 = sunday 8 = allweek
    8
    830 baht
