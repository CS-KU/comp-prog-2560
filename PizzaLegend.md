#Pizza Legend
ให้เขียนโปรแกรมสำหรับร้านขายพิซซาที่สามารถสั่งได้ 1000 ครั้ง อย่างไรก็ได้ตามต้องการ
ซึ่งขายพิซซ่าสามขนาด ได้แก่ ขนาดเล็ก(S) กลาง(M) และใหญ่(L) 
ราคา 100 บาท 150 บาท และ 200 บาท ตามลำดับ
และเครื่องต่างๆ ได้แก่ พริก(Chilli) มะเขือเทศ(Tomato) เบคอน(Bacon) กุ้ง(Shrimp) 
ราคา 10 บาท20 บาท 30 บาท และ 40 บาท ตามลำดับ
ให้รับค่าคำสั่งต่างๆทั้งขนาดพิซซ่า เครื่องต่างๆได้อย่างไม่จำกัด จนกว่าจะพิมพ์ค่า 0
นอกจากนี้ยังสามารถสั่งกี่ถาดก็ได้ จนกว่าจะพิมพ์ค่า 0
เมื่อจบการสั่งซื้อ โปรแกรมจะคำนวณเงินทั้งหมดที่ต้องจ่ายออกมาและรหัสรายการสั่งทั้งหมด โดยรหัสแต่ละรายการ คือ ขนาดเล็ก = S กลาง = M และใหญ่ = L 
พริก(Chilli) = c มะเขือเทศ(Tomato) = t เบคอน(Bacon) = b กุ้ง(Shrimp) = s
ถ้าสั่งนอกเหนือจากที่กำหนดจะขึ้น “ERROR” และให้สั่งใหม่อีกครั้ง
---
## ตัวอย่าง input/output 1

	Welcome to My Pizza Legend!!
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Select pizza size
	(1=S, 2=M, or 3=L): 1
	Choose what you want to put in the pizza.
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 1
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 2
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 3
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 4
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 0
	1 more needed? (1=yes, 0=no): 0
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	All orders code : S c t b s
	Your order all costs 200 baht.
	Thank you.
---
## ตัวอย่าง input/output 2

	Welcome to My Pizza Legend!!
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Select pizza size
	(1=S, 2=M, or 3=L): 1
	Choose what you want to put in the pizza.
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 2
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 0
	1 more needed? (1=yes, 0=no): 1
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Select pizza size
	(1=S, 2=M, or 3=L): 2
	Choose what you want to put in the pizza.
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 1
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 4
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 0
	1 more needed? (1=yes, 0=no): 1
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Select pizza size
	(1=S, 2=M, or 3=L): 3
	Choose what you want to put in the pizza.
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 4
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 0
	1 more needed? (1=yes, 0=no): 0
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	All orders code : S t M c s L s
	Your order all costs 560 baht.
	Thank you.
---





