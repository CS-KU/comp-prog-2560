##Hell or Heaven game
	<br/>กติกา มีอยู่ว่าให้คุณเลือกเลขที่อยู่ระหว่าง1-6 ถ้านอกเหนือจากเลขนี้ก็จะถูกเตือนและกรอกใหม่ โดยแต่ละเลข 1-50 จะมี


-	**นรก** คือ เดินถอยหลังตามที่โปรแกรมกำหนดอัตโนมัติ
โดยกำหนดเลขต่อไปนี้เป็นเลขนรก
5, 10, 14, 18, 20, 22, 29, 33, 37, 40, 44, 47, 49

	โดยเดินถอยหลังตามลำดับ

	-2, -2, -3, -3, -8, -6, -4, 2, -10, -6, -6, -6, -3

-	**สวรรค์**  คือ เดินข้างหน้าเพิ่มตามที่โปรแกรมกำหนดอัตโนมัติ
โดยกำหนดเลขต่อไปนี้เป็นเลขสวรรค์
6, 7, 13, 24, 28, 35, 45

	โดยเดินหน้าตามลำดับ

	+3, +5, +8, +6,+3, +4, +3
-	**เลข jackpot** คือเลข 32 ได้เดินหน้า 18  ช่องจะถึงเส้นชัยทันที
-	**ช่องว่าง** คือ อยู่ที่เดิม

จะเล่นไปเรื่อยๆจนกว่าจะถึงเส้นชัย คือ 50

พอจบเกมจะบอกว่าคุณได้ทายตัวเลขไปทั้งหมดกี่รอบ

**ข้อมูล Input**

1. รับค่าจำนวนเต็ม ตั้งแต่ 1-6 ไปเรื่ยๆจนกว่าจะถึงเส้นชัย 
<br/>- choose number (1-6) : ตัวเลขที่ทายเข้ามา

2. ถ้าทายเลขนอกเหนือจากนี้จะมีข้อความว่า
<br/>>>> Invalid number, Try again! <<<

**ข้อมูล Output**

1. ถ้าทายโดนเลขสวรรค์ จะมีข้อความว่า 
<br/>Heaven, You go to จำนวนที่ได้ไป stage.
<br/>และบอกว่าปัจจุบันอยู่ตำแหน่งอะไร
<br/>(now you stay stage ตำแหน่งที่อยู่)

2. ถ้าทายโดนเลขนรก จะมีข้อความว่า
<br/>Hell, You back จำนวนที่เดินถอยหลัง stage.
<br/>(now you stay stage ตำแหน่งที่อยู่)

3. ถ้าทายโดนเลขแจ็คพอต จะมีข้อความว่า
<br/>JACKPOT YOU WIN.
<br/>You go to finish.
<br/>(now you stay stage ตำแหน่งที่อยู่)

4. ถ้าไม่โดนอะไรเลย จะมีข้อความว่า
<br/>No hell and heaven.

5. พอทายถึงเลขสุดท้ายจะมีข้อมูลบอกว่าคุณได้ทายไปทั้งหมดกี่รอบ
<br/>You choose จำนวนครั้งที่ทายไป time.


**Example 1**
<br/>- choose number (1-6) : 9
<br/>>>> Invalid number, Try again! <<<
<br/>(now you stay stage 0.)
<br/>
<br/>- choose number (1-6) : -1
<br/>>>> Invalid number, Try again! <<<
<br/>(now you stay stage 0.)
<br/>
<br/>- choose number (1-6) : 1
<br/>No hell and heaven.
<br/>(now you stay stage 1.)
<br/>
<br/>- choose number (1-6) : 6
<br/>Heaven, You go to 5 stage.
<br/>(now you stay stage 12.)
<br/>
<br/>- choose number (1-6) : 1
<br/>Heaven, You go to 8 stage.
<br/>(now you stay stage 21.)
<br/>
<br/>- choose number (1-6) : 4
<br/>No hell and heaven.
<br/>(now you stay stage 25.)
<br/>
<br/>- choose number (1-6) : 3
<br/>Heaven, You go to 3 stage.
<br/>(now you stay stage 31.)
<br/>
<br/>- choose number (1-6) : 2
<br/>Hell, You back 2 stage.
<br/>(now you stay stage 31.)
<br/>
<br/>- choose number (1-6) : 1
<br/>JACKPOT YOU WIN.
<br/>You go to finish.
<br/>(now you stay stage 50.)
<br/>You choose 9 time.

**Example2**
<br/>- choose number (1-6) : 4
<br/>No hell and heaven.
<br/>(now you stay stage 4.)
<br/>
<br/>- choose number (1-6) : 2
<br/>Heaven, You go to 3 stage.
<br/>(now you stay stage 9.)
<br/>
<br/>- choose number (1-6) : 3
<br/>No hell and heaven.
<br/>(now you stay stage 12.)
<br/>
<br/>- choose number (1-6) : 4
<br/>No hell and heaven.
<br/>(now you stay stage 16.)
<br/>
<br/>- choose number (1-6) : 5
<br/>No hell and heaven.
<br/>(now you stay stage 21.)
<br/>
<br/>- choose number (1-6) : 2
<br/>No hell and heaven.
<br/>(now you stay stage 23.)
<br/>
<br/>- choose number (1-6) : 11
<br/>>>> Invalid number, Try again! <<<
<br/>(now you stay stage 23.)
<br/>
<br/>- choose number (1-6) : 2
<br/>No hell and heaven.
<br/>(now you stay stage 25.)
<br/>
<br/>- choose number (1-6) : 3
<br/>Heaven, You go to 3 stage.
<br/>(now you stay stage 31.)
<br/>
<br/>- choose number (1-6) : 4
<br/>Heaven, You go to 4 stage.
<br/>(now you stay stage 39.)
<br/>
<br/>- choose number (1-6) : 5
<br/>Hell, You back 6 stage.
<br/>(now you stay stage 38.)
<br/>
<br/>- choose number (1-6) : 7
<br/>>>> Invalid number, Try again! <<<
<br/>(now you stay stage 38.)
<br/>
<br/>- choose number (1-6) : 4
<br/>No hell and heaven.
<br/>(now you stay stage 42.)
<br/>
<br/>- choose number (1-6) : 5
<br/>Hell, You back 6 stage.
<br/>(now you stay stage 41.)
<br/>
<br/>- choose number (1-6) : 6
<br/>Hell, You back 6 stage.
<br/>(now you stay stage 41.)
<br/>
<br/>- choose number (1-6) : 2
<br/>No hell and heaven.
<br/>(now you stay stage 43.)
<br/>
<br/>- choose number (1-6) : 1
<br/>Hell, You back 6 stage.
<br/>(now you stay stage 38.)
<br/>
<br/>- choose number (1-6) : 6
<br/>Hell, You back 6 stage.
<br/>(now you stay stage 38.)
<br/>
<br/>- choose number (1-6) : 5
<br/>No hell and heaven.
<br/>(now you stay stage 43.)
<br/>
<br/>- choose number (1-6) : 2
<br/>Heaven, You go to 3 stage.
<br/>(now you stay stage 48.)
<br/>- choose number (1-6) : 2
<br/>>>> You win <<<
<br/>(now you stay stage 50.)
<br/>
<br/>You choose 21 time.
