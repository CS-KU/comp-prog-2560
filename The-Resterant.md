# The Restaurant
ร้านอาหารแห่งหนึ่ง มาจ้างให้คุณเขียนโปรแกรมเพื่อให้ลูกค้าสั่งอาหารตามเมนูหลัก และเมนูรองดังนี้ 1.Dessert => 1. Cake 2. Ice Cream 3. Pudding ราคา 40, 30, 50 บาท ตามลำดับ
2.Food => 1. Burger 2. Chicken Fried 3. Salad ราคา 60, 100, 40 บาท ตามลำดับ
3.Drink => 1. Cola 2. Orange Juice 3. Tea ราคา 20, 20, 10 บาท ตามลำดับ
ซึ่งทางร้านจะให้ลูกค้าสั่งเมนูเรื่อยๆ จนกว่าลูกค้าจะพอใจ เมื่อลูกค้าพอใจเมื่อตอบ “0”
และถ้าลูกค้ามีบัตรสมาชิก จะลดค่าอาหาร 15% ของราคาทั้งหมด

**ข้อมูลเข้า**
* เมนูหลักของอาหารเป็นจำนวนเต็มของเมนู ในบรรทัดแรก เมื่อลูกค้าตอบ “0” มา จะหยุดรับเมนู
* เมนูรองของเมนูหลักเป็นจำนวนเต็มของเมนู ในบรรทัดต่อมา
* บัตรสมาชิกของลูกค้า หลังจากลูกค้าโปรแกรมหยุดรับเมนูแล้ว

**ข้อมูลออก**
* ค่าอาหารทศนิยม 2 ตำแหน่ง #หากมีคำตอบของแต่ละข้อไม่มีในตัวเลือกให้แสดงข้อความ “ERROR!” และรับค่าใหม่ และหากลูกค้าตอบ “0” ทั้งที่ไม่ได้สั่งอาหารไม่ต้องถามถึงบัตรสมาชิก 

**ตัวอย่าง Input/Output 1**

    ---Welcome---
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 1
    Enter Sub Menu(1. Cake 2. Ice Cream 3. Pudding): 1
    ----------
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 1
    Enter Sub Menu(1. Cake 2. Ice Cream 3. Pudding): 2
    ----------
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 1
    Enter Sub Menu(1. Cake 2. Ice Cream 3. Pudding): 3
    ----------
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 0
    Have a member card: (1. NO 2. Yes): 1
    Your cost is 120.00 Bath
---
**ตัวอย่าง Input/Output 2**

    ---Welcome---
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 1
    Enter Sub Menu(1. Cake 2. Ice Cream 3. Pudding): 1
    ----------
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 2
    Enter Sub Menu(1. Burger 2. Chicken Fried 3. Salad): 2
    ----------
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 3
    Enter Sub Menu(1. Cola 2. Orange Juice 3. Tea): 3
    ----------
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 0
    Have a member card: (1. NO 2. Yes): 2
    Your cost is 127.50 Bath
---
**ตัวอย่าง Input/Output 3**

    ---Welcome---
    Enter Main Menu(1. Dessert 2. Food 3. Drink): 0
    Your cost is 0.00 Bath
---