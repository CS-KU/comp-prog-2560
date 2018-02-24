#Pizza eiei
ให้เขียนโปรแกรมสำหรับร้านขายพิซซาที่สามารถสั่งเครื่องที่มีได้เท่าไหร่ก็ได้ตามต้องการ
ซึ่งขายพิซซ่าสามขนาด ได้แก่ ขนาดเล็ก(s) กลาง(m) และใหญ่(l) 
ราคา 100 บาท 150 บาท และ 200 บาท ตามลำดับ
และเครื่องต่างๆ ได้แก่ พริก(Chilli) มะเขือเทศ(Tomato) เบคอน(Bacon) กุ้ง(Shrimp) 
ราคา 10 บาท20 บาท 30 บาท และ 40 บาท ตามลำดับ
ให้รับค่าคำสั่งต่างๆทั้งขนาดพิซซ่า เครื่องต่างๆได้อย่างไม่จำกัด จนกว่าจะพิมพ์ค่า 0
นอกจากนี้ยังสามารถสั่งกี่ถาดก็ได้ จนกว่าจะพิมพ์ค่า 0
เมื่อจบการสั่งซื้อ โปรแกรมจะคำนวณเงินทั้งหมดที่ต้องจ่ายออกมา
ถ้าสั่งนอกเหนือจากที่กำหนดจะขึ้น “ERROR” และให้สั่งใหม่อีกครั้ง
---
## ตัวอย่าง input/output 1

	Welcome to My Pizza eiei!!
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Select pizza size
	(1=s, 2=m, or 3=l): 0
	ERROR
	Select pizza size
	(1=s, 2=m, or 3=l): 3
	Choose what you want to put in the pizza.
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 4
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 0
	1 more needed? (1=yes, 0=no): 3
	ERROR
	1 more needed? (1=yes, 0=no): 0
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Your order all costs 240 baht.
	Thank you.
---
## ตัวอย่าง input/output 2

	Welcome to My Pizza eiei!!
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Select pizza size
	(1=s, 2=m, or 3=l): 3
	Choose what you want to put in the pizza.
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 0
	1 more needed? (1=yes, 0=no): 1
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Select pizza size
	(1=s, 2=m, or 3=l): 1
	Choose what you want to put in the pizza.
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 0
	1 more needed? (1=yes, 0=no): 1
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Select pizza size
	(1=s, 2=m, or 3=l): 2
	Choose what you want to put in the pizza.
	(1)Chilli (2)Tomato (3)Bacon (4)Shrimp (1 piece)
	(Press 0 to end.): 0
	1 more needed? (1=yes, 0=no): 0
	~~~~~~~~~~~~~~~~~~~~~~~~~~
	Your order all costs 450 baht.
	Thank you.
---





