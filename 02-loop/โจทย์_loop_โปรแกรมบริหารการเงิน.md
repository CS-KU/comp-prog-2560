#โปรแกรมบริหารการเงิน แบบง่าย   
by 6010405092

	เด็กคนหนึ่งต้องการที่จะเก็บเงินจำนวนหนึ่ง แต่ด้วยความที่เป็นเด็กที่ใช้จ่ายเงินเก่ง และ บ่อย จึงเก็บเงินไม่ได้ตามเป้าหมายสักที ทำให้ เด็กคนนี เครียดมากและได้นำปัญหาเหล่านี้ ไปปรึกษากับแฟนบ่อยๆ  ปรึกษาบ่อยเข้าแฟนชักจะรำคาญ พอดีช่วงนั้นก่อนวันวาเลนไทน์ 2วัน แฟนจึง ตัดสินใจทำโปรแกรมเพื่อช่วยให้เด็กคนนั้นมีความดึงดูดที่อยากจะเก็บเงิน  และ เป็นของขวัญวันวาเลนไทน์ด้วย  โดยโปรแกรมมีรายละเอียดดังนี้ เมื่อรันโปรแกรม โปรแกรมจะแสดงว่า
Please give me some data to start program money control.

	จากนั้น กดปุ่มใดก็ได้บนคีย์บอร์ด เพื่อทำงานต่อไปดังนี้
	
What's your name? 
==> kitpavin
How much money do you have now? 
==> 50
What is your target? 
==> 300
-----------Thank you----------- 
----(press any key to next)----

	หลังจากใส่ ชื่อ จำนวนเงินที่มีอยู่ตอนนี้ และ เงินเป้าหมายที่ต้องการจะสะสมแล้ว ก็ กดปุ่มใดก็ได้บนคีย์บอร์ด เพื่อทำงานต่อไป
Income or expenditure (press (1) for income, (2) for expenditure): 1 
How much income do you have?: 40 
kitpavin has 90.00 baht.
\**** 
\--------------- 
(Press 'e' to exit, Any key to continue)

	โปรแกรมจะถามว่า มีรายรับ หรือ รายจ่าย โดยถ้ามีรายรับ กด 1, รายจ่าย กด 2 โปรแกรมจะถามว่ารายรับ หรือ รายจ่ายนั้นกี่บาท  จากนั้นแสดงว่า เหลือเงินเท่าใด และ แสดงหลอดเป้าหมายแบบง่ายๆ  โดย $ แทนเงินที่มีอยู่ (($) 1 ตัวต่อ 20 บาท แต่ถ้า เงินมีอยู่น้อยกว่า 20 ให้ ($) 1 ตัวต่อ 5 บาทแทน) (-)  แทนเงินเป้าหมาย ((-) 1 ตัวต่อ 20 บาท แต่ถ้า เงินทีjมีอยู่น้อยกว่า 20 ให้ (-) 1 ตัวต่อ 5 บาทแทน)แต่ถ้าเงินติดลบให้แสดงเหมือนเงิน 0 บาท

ตัวอย่าง
	1.	มีเงิน 50 บาท เป้าหมาย 500 จะแสดง
**
\------------------------- 
	2.	50 จะแทนด้วย ($) สองตัว (เศษบัดทิhง),  500 จะแทนด้วย (-) 25 ตัว
ถ้า มีเงิน -5 บาท เป้าหมาย 200 จะแสดง

\----------------------------------------
-5 แทนด้วย ($) 0 ตัว, 200 แทนด้วย  (-) 40 ตัว เนื่องจากเปลี่ยนสเกลเป็น  (-) ละ 5 แล้ว ซึ่งโปรแกรมจะถามเช่นนี้ไปเรื่อยๆ กว่าผู้ใช้จะกด  ‘e’ จะแสดงข้อความว่า    
---------------Thank you---------------
แล้วจบโปรแกรม   

	เพื่อความเข้าใจที่มากขึ้น ดูตัวอย่างการทำงานต่อไปนี้
	
Please give me some data to start program money control.
----------------(press any key to next)---------------- 
What's your name? 
==> Zen 
How much money do you have now? 
==> 50 
What is your target? 
==> 350 
-----------Thank you----------- 

Income or expenditure (press (1) for income, (2) for expenditure): 1 
How much income do you have?: 165 
Zen has 215.00 baht. 
\**********
\----------------- 
(Press 'e' to exit, Any key to continue)

Income or expenditure (press (1) for income, (2) for expenditure): 1 
How much income do you have?: 195 
Zen has 410.00 baht.
\******************** 
\----------------- 
(Press 'e' to exit, Any key to continue)

Income or expenditure (press (1) for income, (2) for expenditure): 2 
How much expenditure do you have?: 403 
Zen has 7.00 baht.
$ 
\---------------------------------------------------------------------- 
(Press 'e' to exit, Any key to continue)

Income or expenditure (press (1) for income, (2) for expenditure): 2 
How much expenditure do you have?: 10 
Zen has -3.00 baht.

\---------------------------------------------------------------------- 
(Press 'e' to exit, Any key to continue)

Income or expenditure (press (1) for income, (2) for expenditure): 1
 How much income do you have?: 200 
Zen has 197.00 baht.
\********* 
\----------------- 
(Press 'e' to exit, Any key to continue)
---------------Thank you---------------

	หมายเหตุ  
	1 . ถ้าสังเกตให้ดี จะพบว่า ถ้าเรากดปุ่มอะไรก็ได้เพื่อข้ามไปยัง step ถัดไป ปุ่มที่เรากดจะไม่แสดงขึ้นบนจอ อักษร ‘e’ ที่เรากดเพื่อที่จะจบ โปรแกรมก็เช่นกัน
	2 . โปรแกรมนี้สามารถคำนวณเงินให้ได้แค่ 500 รอบต่อการทำงาน 1 ครั้ง

