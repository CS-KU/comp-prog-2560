#include <stdio.h>
int main(){
    int n,i,j;
    printf("Enter n: ");
    scanf("%d",&n);
    for (i=1;i<n;i++){
        for (j=1;j<=i;j++){
            if (j%2==0)
                printf("x");
            else 
                printf("-");
        }printf("\n");
    }for (;i>0;i--){
        for (j=1;j<=i;j++){
            if (j%2==0)
                printf("x");
            else 
                printf("-");
        }printf("\n");
    }
}## Happy Farm
โจทย์ปัญหา
จากความทรงจำในอดีตที่เคยมาเยี่ยมฟาร์มของคุณปู่ของเราและได้จากไปจากหมู่บ้าน จนวันนี้คุณได้กลับมายังหมู่บ้านนี้อีกครั้งและต้องเข้ามาจัดการกับฟาร์มของเราซึ่งสืบทอดมาจากคุณปู่ด้วยตัวเองแล้วใน Happy Farm 
ภารกิจของคุณการเขียนโค้ดเกมเกี่ยวกับ ฟาร์มปศุสัตว์
โดยมีจุดเริ่มต้นของคุณคือที่บ้าน จากนั้นจะมีเมนูให้เลือก

( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit )

•	Bed : ไปที่เตียงนอน
•	Farm : ไปที่ฟาร์ม
•	City : ไปในเมือง
•	Sea : ไปที่ทะเล
•	Check : เช็คข้อมูลตัวละคร
•	Exit : ออกจากเกม

กรณีที่เลือก Check จะขึ้นข้อมูลมาให้ดู
	 
	Baht : จะขึ้นจำนวนเงินมาให้ โดยเริ่มแรกจะมีเงินมาให้ 500
	Fish : จำนวนปลาที่อยู่กับคุณ โดยเริ่มแรกจะมีค่าเป็น 0
	Fish pond : จำนวนปลาในบ่อ โดยเริ่มแรกจะมีค่าเป็น 0
	Chicken : จำนวนไก่ โดยเริ่มแรกจะมีค่าเป็น 0
	Egg : จำนวนไข่ไก่ที่อยู่กับคุณ โดยเริ่มแรกจะมีค่าเป็น 0
	Fodder chicken : จำนวนอาหารไก่ โดยเริ่มแรกจะมีค่าเป็น 0
	Cow : จำนวนวัว โดยเริ่มแรกจะมีค่าเป็น 0
	Milk : จำนวนนมที่อยู่กับคุณ โดยเริ่มแรกจะมีค่าเป็น 0
	Sheep : จำนวนแกะ โดยเริ่มแรกจะมีค่าเป็น 0
	Wool : จำขนแกะที่อยู่กับคุณ โดยเริ่มแรกจะมีค่าเป็น 0
	Fodder : จำนวนอาหารวัวและแกะ โดยเริ่มแรกจะมีค่าเป็น 0
	Hungry : ปริมาณความหิว โดยเริ่มแรกจะมีค่าเป็น 15 

	***ความหิวสูงสุดได้ไม่เกิน 15

กรณีที่เลือก Bed จากนั้นจะมีเมนูให้เลือก
	
	( |Y|es / |N|o)

	กรณีที่เลือก Yes จะขึ้นข้อมูลมาให้ดูแบบเดียวกับเช็ค แต่ค่าความหิวจะเพิ่มขึ้น 10

	กรณีที่เลือก No กลับไปยังบ้าน



กรณีที่เลือก Farm จากนั้นจะมีเมนูให้เลือก

( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit )

•	Henhouse : ไปที่เล้าไก่
•	Fish pond : ไปที่บ่อปลา
•	Cow and sheep : ไปที่โรงเลี้ยงวัวและแกะ
•	Exit :  กลับไปที่บ้าน

กรณีที่เลือก Henhouse หรือ Cow and sheep จากนั้นจะมีเมนูให้เลือก

( |G|ive / |K|eep / |E|xit )

•	Give : ให้อาหารสัตว์
•	Keep : เก็บผล
•	Exit : กลับไปที่ฟาร์ม

*** กรณีที่เลือก Keep ผลผลิตจะสามารถเก็บในวันถัดไปหลังจากให้อาหารแล้ว ปริมาณผลขึ้นอยู่กับเงื่อนไข 
กรณีอาหารมากกว่าหรือเท่ากับสัตว์ ผลผลิตที่ได้จะได้จะมีปริมาณเท่ากับสัตว์ที่เลี้ยง
กรณีอาหารน้อยกว่าสัตว์ ผลผลิตที่ได้จะได้จะมีปริมาณเท่ากับอาหารที่ให้

*** กรณีที่เลือก Cow and sheep แล้วเลือกคำสั่ง Keep จะมีตัวเลือกขึ้นมาให้เลือก
	
		( |C|ow / |S|heep / |E|xit )

•	Cow :  เก็บนม
•	Sheep : เก็บขนแกะ
•	Exit : กลับไปยังคำสั่ง Cow and sheep

*** ขนแกะจะสามารถเก็บได้ก็ต่อเมื่อเลี้ยงไปได้ 15 วันต่อ 1 ครั้ง เท่านั้น

กรณีที่เลือก Fish pond ต่อจากนั้นจะมีเมนูให้เลือก
	
( |R|elease / |F|ishing / |E|xit )

•	Release : ปล่อยปลาลงบ่อ
•	Fishing : จับปลา
•	Exit : กลับไปที่ฟาร์ม

*** 	ทุกครั้งที่ทำกิจกรรม ค่าความหิวจะลดลงที่ 1 ถ้าค่าความหิวเป็น 0 จะไม่สามารถจะทำกิจกรรมภายในฟาร์ม หรือ ตกปลาได้
กรณีที่เลือก City จากนั้นจะมีเมนูให้เลือก

	( |R|ick / |M|ay / |A|nn / |E|xit )

•	Rick : ร้านขายไก่
•	May : ร้านขายวัว และ แกะ
•	Ann : ร้านขายอาหาร
•	Exit : กลับไปยังบ้าน

กรณีที่เลือก Rick  จากนั้นจะมีเมนูให้เลือก
	
	( |B|uy / |S|ell / |F|odder chicken / |E|xit )

•	Buy : ขายไก่  ราคา 500
•	Sell : ซื้อไก่  ราคา 250
•	Fodder chicken : ขายอาหารไก่ ราคา 5
•	Exit :  กลับไปที่เมือง

กรณีที่เลือก May จากนั้นจะมีเมนูให้เลือก
	
	( |B|uy / |S|ell / |F|odder / |E|xit )

•	Buy : ขายสัตว์
•	Sell : ซื้อสัตว์
•	Fodder chicken : ขายอาหาร ราคา 10
•	Exit :  กลับไปที่เมือง

*** กรณีที่เลือก Buy หรือ Sell จะมีตัวเลือกขึ้นมาให้เลือก
	
		( |C|ow / |S|heep )

•	Cow :  Buy ราคา 5000 กับ Sell ราคา 2500  
•	Sheep : Buy ราคา 4000 กับ Sell ราคา  2000

กรณีที่เลือก Ann จากนั้นจะมีเมนูให้เลือก
		
		( |C|ake / |W|ater / |F|ried rice / |E|xit )
	
•	Cake : ราคา 100 เพิ่มค่าความหิว 3
•	Water : ราคา 20 เพิ่มค่าความหิว 1
•	Fried rice : ราคา 150 เพิ่มค่าความหิว 5

***ค่าเงินห้ามติดลบ

กรณีที่เลือก Sea จากนั้นจะมีเมนูให้เลือก
	
	( |S|ea / |Z|ack / |E|xit )

	Sea : ไปตกปลา
	Zack : ร้านรับซื้อของ
	Exit : กลับไปยังบ้าน

	กรณีที่เลือก Sea จากนั้นจะมีเมนูให้เลือกว่าตกปลาหรือเปล่า ถ้าจะตกปลาให้ทำการสุ่มตัวเลข ถ้าเป็นเลขคี่ จะได้ปลาเพิ่ม 1 ตัว แต่ถ้าเป็นเลขคู่ จะไม่ได้อะไรเลย

	กรณีที่เลือก Zack จากนั้นจะมีเมนูให้เลือก

		( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o )

•	Egg : ต้องการขายไข่ ราคา 25
•	Fish : ต้องการขายปลา ราคา 20
•	Milk : ต้องการขายนม ราคา 150
•	Wool : ต้องการขายขนแกะ ราคา 250
•	No :  ออกจากร้าน

***  รวมเงื่อนไขตัวพิมพ์เล็ก  (lower case), ตัวพิมพ์ใหญ่ (upper case)

## ตัวอย่าง input/output

Test Case 1
```
~~~~~~~~~~~~~~~~~~~~~~~ Wecome to Happy Farm ~~~~~~~~~~~~~~~~~~~~~~~
Day : 1
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): a
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): s
Wecome to Sea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |S|ea / |Z|ack / |E|xit ): s
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 2
Fail.
Do you want to fish ( |Y|es / |N|o ): n
Do you want to go ( |S|ea / |Z|ack / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): h
--------------------------------------------------------------------
Baht : 500
Fish : 1
Fish pond : 0
Chicken : 0
Egg : 0
Fodder chicken : 0
Cow : 0
Milk : 0
Sheep : 0
Wool : 0
Fodder : 0
Hungry : 13
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): s
Welcome to Sea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |S|ea / |Z|ack / |E|xit ): z
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): f
amount : 1
receive money : 20
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): f
amount : 1
Insufficient Product.
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): n
Do you want to go ( |S|ea / |Z|ack / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): h
--------------------------------------------------------------------
Baht : 520
Fish : 0
Fish pond : 0
Chicken : 0
Egg : 0
Fodder chicken : 0
Cow : 0
Milk : 0
Sheep : 0
Wool : 0
Fodder : 0
Hungry : 13
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): e
--------------------------------------------------------------------
-------------------------- See you again ---------------------------
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ Bye bye ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```
Test Case 2
```
~~~~~~~~~~~~~~~~~~~~~~~ Welcome to Happy Farm ~~~~~~~~~~~~~~~~~~~~~~~
Day : 1
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): c
Welcome to City
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |R|ick / |M|ay / |A|nn / |E|xit ): r
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): b
Thank You.
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): b
Your money is not enough.
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): f
Amount of feed : 1
Your money is not enough.
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): e
Do you want to go ( |R|ick / |M|ay / |A|nn / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): s
Wecome to Sea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |S|ea / |Z|ack / |E|xit ): s
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): n
Do you want to go ( |S|ea / |Z|ack / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): c
Welcome to City
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |R|ick / |M|ay / |A|nn / |E|xit ): r
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): e
Do you want to go ( |R|ick / |M|ay / |A|nn / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): z
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): s
Welcome to Sea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |S|ea / |Z|ack / |E|xit ): z
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): f
amount : 6
receive money : 120
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): n
Do you want to go ( |S|ea / |Z|ack / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): c
Welcome to City
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |R|ick / |M|ay / |A|nn / |E|xit ): r
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): f
Amount of feed : 10
Thank You.
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): e
Do you want to go ( |R|ick / |M|ay / |A|nn / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): f
Welcome to Farm
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  h
What do you want to do ( |G|ive / |K|eep / |E|xit ): g
Amount of feed chicken meal : 1
What do you want to do ( |G|ive / |K|eep / |E|xit ): k
What do you want to do ( |G|ive / |K|eep / |E|xit ): e
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): b
Do you want to sleep ( |Y|es / |N|o): y
-------------------------------------------------------------------
Baht : 70
Fish : 0
Fish pond : 0
Chicken : 1
Egg : 0
Fodder chicken : 9
Cow : 0
Milk : 0
Sheep : 0
Wool : 0
Fodder : 0
Hungry : 15
--------------------------------------------------------------------
Day : 2
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): f
Welcome to Farm
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  h
What do you want to do ( |G|ive / |K|eep / |E|xit ): g
Amount of feed chicken meal : 2
What do you want to do ( |G|ive / |K|eep / |E|xit ): k
What do you want to do ( |G|ive / |K|eep / |E|xit ): e
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): b
Do you want to sleep ( |Y|es / |N|o): y
-------------------------------------------------------------------
Baht : 70
Fish : 0
Fish pond : 0
Chicken : 1
Egg : 1
Fodder chicken : 7
Cow : 0
Milk : 0
Sheep : 0
Wool : 0
Fodder : 0
Hungry : 15
--------------------------------------------------------------------
Day : 3
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): f
Welcome to Farm
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  h
What do you want to do ( |G|ive / |K|eep / |E|xit ): k
What do you want to do ( |G|ive / |K|eep / |E|xit ): e
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  s
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): s
Welcome to Sea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |S|ea / |Z|ack / |E|xit ): s
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Do you want to fish ( |Y|es / |N|o ): n
Do you want to go ( |S|ea / |Z|ack / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): b
Do you want to sleep ( |Y|es / |N|o): y
-------------------------------------------------------------------
Baht : 70
Fish : 14
Fish pond : 0
Chicken : 1
Egg : 2
Fodder chicken : 7
Cow : 0
Milk : 0
Sheep : 0
Wool : 0
Fodder : 0
Hungry : 10
--------------------------------------------------------------------
Day : 4
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): f
Welcome to Farm
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  h
What do you want to do ( |G|ive / |K|eep / |E|xit ): k
What do you want to do ( |G|ive / |K|eep / |E|xit ): e
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): s
Welcome to Sea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |S|ea / |Z|ack / |E|xit ): s
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Random fish : 1
Success.
Do you want to fish ( |Y|es / |N|o ): y
Do you want to fish ( |Y|es / |N|o ): y
Do you want to fish ( |Y|es / |N|o ): n
Do you want to go ( |S|ea / |Z|ack / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): b
Do you want to sleep ( |Y|es / |N|o): y
-------------------------------------------------------------------
Baht : 70
Fish : 24
Fish pond : 0
Chicken : 1
Egg : 2
Fodder chicken : 7
Cow : 0
Milk : 0
Sheep : 0
Wool : 0
Fodder : 0
Hungry : 10
--------------------------------------------------------------------
Day : 5
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): f
Welcome to Farm
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  h
What do you want to do ( |G|ive / |K|eep / |E|xit ): g
Amount of feed chicken meal : 1
What do you want to do ( |G|ive / |K|eep / |E|xit ): e
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): s
Welcome to Sea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |S|ea / |Z|ack / |E|xit ): z
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): e
amount : 1
receive money : 25
Do you want to go ( |S|ea / |Z|ack / |E|xit ): z
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): f
amount : 2
receive money : 40
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): f
amount : 20
receive money : 400
What do you want to sell ( |E|gg / |F|ish / |M|ilk / |W|ool / |N|o ): n
Do you want to go ( |S|ea / |Z|ack / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): b
Do you want to sleep ( |Y|es / |N|o): y
-------------------------------------------------------------------
Baht : 535
Fish : 2
Fish pond : 0
Chicken : 1
Egg : 1
Fodder chicken : 6
Cow : 0
Milk : 0
Sheep : 0
Wool : 0
Fodder : 0
Hungry : 15
--------------------------------------------------------------------
Day : 6
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): c
Welcome to City
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |R|ick / |M|ay / |A|nn / |E|xit ): r
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): b
Thank You.
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): f
Amount of feed : 5
Thank You.
What do you want to do ( |B|uy / |S|ell / |F|odder chicken / |E|xit ): e
Do you want to go ( |R|ick / |M|ay / |A|nn / |E|xit ): e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): f
Welcome to Farm
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  h
What do you want to do ( |G|ive / |K|eep / |E|xit ): k
What do you want to do ( |G|ive / |K|eep / |E|xit ): g
Amount of feed chicken meal : 2
What do you want to do ( |G|ive / |K|eep / |E|xit ): e
Do you want to go ( |H|enhouse / |F|ish pond / |C|ow and sheep / |E|xit ):  e
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): b
Do you want to sleep ( |Y|es / |N|o): y
-------------------------------------------------------------------
Baht : 10
Fish : 2
Fish pond : 0
Chicken : 2
Egg : 2
Fodder chicken : 9
Cow : 0
Milk : 0
Sheep : 0
Wool : 0
Fodder : 0
Hungry : 15
--------------------------------------------------------------------
Day : 7
--------------------------------------------------------------------
Now you are in the house
Do you want to go ( |B|ed / |F|arm / |C|ity / |S|ea / c|H|eck / |E|xit ): e
--------------------------------------------------------------------
-------------------------- See you again ---------------------------
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ Bye bye ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```