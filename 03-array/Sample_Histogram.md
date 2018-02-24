# Sample Histogram

**ฮิสโตแกรม (Histogram)** คือ กราฟแท่งแบบเฉพาะที่แสดงความสัมพันธ์ระหว่างข้อมูลเป็นหมวดหมู่ เพื่อดูการกระจายของข้อมูล จงเขียนโปรแกรมรับค่าจำนวนตัวเลข 10 ค่า และแสดงผลจำนวนสมาชิกของ Array ค่า index ของแต่ละสมาชิก และแสดงผลค่าที่รับในรูปแบบกราฟแบบ Bar Chart โดยใช้ * แทนจำนวนตัวเลขดังตัวอย่าง Test Case ต่อไปนี้

**หมายเหตุ** : ค่าที่รับจะต้องเป็นจำนวนเต็มบวกที่มากกว่า 0 เท่านั้น หากค่าที่รับมีค่าน้อยกว่า ให้แสดงข้อความ **Please enter value of num again.** และรับค่าใหม่อีกครั้ง

## Test Case 1
    Enter value of num[0]:  1
    Enter value of num[1]:  2
    Enter value of num[2]:  3
    Enter value of num[3]:  4
    Enter value of num[4]:  5
    Enter value of num[5]:  6
    Enter value of num[6]:  7
    Enter value of num[7]:  8
    Enter value of num[8]:  9
    Enter value of num[9]:  10

    Element/index          Value          Histogram

          0                  1            *
          1                  2            **
          2                  3            ***
          3                  4            ****
          4                  5            *****
          5                  6            ******
          6                  7            *******
          7                  8            ********
          8                  9            *********
          9                 10            **********

## Test Case 2
    Enter value of num[0]:  2
    Enter value of num[1]:  0
    Please enter value of num again.
    Enter value of num[1]:  4
    Enter value of num[2]:  6
    Enter value of num[3]:  8
    Enter value of num[4]:  9
    Enter value of num[5]:  7
    Enter value of num[6]:  5
    Enter value of num[7]:  3
    Enter value of num[8]:  -5
    Please enter value of num again.
    Enter value of num[8]:  4
    Enter value of num[9]:  2

    Element/index          Value          Histogram
          0                  2            **
          1                  4            ****
          2                  6            ******
          3                  8            ********
          4                  9            *********
          5                  7            *******
          6                  5            *****
          7                  3            ***
          8                  4            ****
          9                  2            **