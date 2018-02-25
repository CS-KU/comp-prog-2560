## Hell or Heaven game

กติกา มีอยู่ว่าให้คุณเลือกเลขที่อยู่ระหว่าง1-6 ถ้านอกเหนือจากเลขนี้ก็จะถูกเตือนและกรอกใหม่ โดยแต่ละเลข 1-50 จะมี


-   **นรก** คือ เดินถอยหลังตามที่โปรแกรมกำหนดอัตโนมัติ
โดยกำหนดเลขต่อไปนี้เป็นเลขนรก
5, 10, 14, 18, 20, 22, 29, 33, 37, 40, 44, 47, 49

	โดยเดินถอยหลังตามลำดับ

	-2, -2, -3, -3, -8, -6, -4, -2, -10, -6, -6, -6, -3

-   **สวรรค์**  คือ เดินข้างหน้าเพิ่มตามที่โปรแกรมกำหนดอัตโนมัติ
โดยกำหนดเลขต่อไปนี้เป็นเลขสวรรค์
6, 7, 13, 24, 28, 35, 45

	โดยเดินหน้าตามลำดับ

	+3, +5, +8, +6, +3, +4, +3
-   **เลข jackpot** คือเลข 32 ได้เดินหน้า 18  ช่องจะถึงเส้นชัยทันที
-   **ช่องว่าง** คือ อยู่ที่เดิม

จะเล่นไปเรื่อยๆ จนกว่าจะถึงเส้นชัย คือ 50

พอจบเกมจะบอกว่าคุณได้ทายตัวเลขไปทั้งหมดกี่รอบ

**ข้อมูล Input**

1.  รับค่าจำนวนเต็ม ตั้งแต่ 1-6 ไปเรื่ยๆจนกว่าจะถึงเส้นชัย
    -   `choose number (1-6): ` ตัวเลขที่ทายเข้ามา

2. ถ้าทายเลขนอกเหนือจากนี้จะมีข้อความว่า
`>>> Invalid number, Try again! <<<`

**ข้อมูล Output**

1.  ถ้าทายโดนเลขสวรรค์ จะมีข้อความว่า
Heaven, You go to จำนวนที่ได้ไป stage.
และบอกว่าปัจจุบันอยู่ตำแหน่งอะไร
(now you stay stage ตำแหน่งที่อยู่)

2.  ถ้าทายโดนเลขนรก จะมีข้อความว่า
Hell, You back จำนวนที่เดินถอยหลัง stage.
(now you stay stage ตำแหน่งที่อยู่)

3.  ถ้าทายโดนเลขแจ็คพอต จะมีข้อความว่า
JACKPOT YOU WIN.
You go to finish.
(now you stay stage ตำแหน่งที่อยู่)

4.  ถ้าไม่โดนอะไรเลย จะมีข้อความว่า
No hell and heaven.

5.  พอทายถึงเลขสุดท้ายจะมีข้อมูลบอกว่าคุณได้ทายไปทั้งหมดกี่รอบ
You choose จำนวนครั้งที่ทายไป time.


**Example 1**
```
choose number (1-6) : 9
>>> Invalid number, Try again! <<<
(now you stay stage 0.)

choose number (1-6) : -1
>>> Invalid number, Try again! <<<
(now you stay stage 0.)

choose number (1-6) : 1
No hell and heaven.
(now you stay stage 1.)

choose number (1-6) : 6
Heaven, You go to 5 stage.
(now you stay stage 12.)

choose number (1-6) : 1
Heaven, You go to 8 stage.
(now you stay stage 21.)

choose number (1-6) : 4
No hell and heaven.
(now you stay stage 25.)

choose number (1-6) : 3
Heaven, You go to 3 stage.
(now you stay stage 31.)

choose number (1-6) : 2
Hell, You back 2 stage.
(now you stay stage 31.)

choose number (1-6) : 1
JACKPOT YOU WIN.
You go to finish.
(now you stay stage 50.)

You choose 9 time.
```

**Example2**

```
choose number (1-6) : 4
No hell and heaven.
(now you stay stage 4.)

choose number (1-6) : 2
Heaven, You go to 3 stage.
(now you stay stage 9.)

choose number (1-6) : 3
No hell and heaven.
(now you stay stage 12.)

choose number (1-6) : 4
No hell and heaven.
(now you stay stage 16.)

choose number (1-6) : 5
No hell and heaven.
(now you stay stage 21.)

choose number (1-6) : 2
No hell and heaven.
(now you stay stage 23.)

choose number (1-6) : 11
>>> Invalid number, Try again! <<<
(now you stay stage 23.)

choose number (1-6) : 2
No hell and heaven.
(now you stay stage 25.)

choose number (1-6) : 3
Heaven, You go to 3 stage.
(now you stay stage 31.)

choose number (1-6) : 4
Heaven, You go to 4 stage.
(now you stay stage 39.)

choose number (1-6) : 5
Hell, You back 6 stage.
(now you stay stage 38.)

choose number (1-6) : 7
>>> Invalid number, Try again! <<<
(now you stay stage 38.)

choose number (1-6) : 4
No hell and heaven.
(now you stay stage 42.)

choose number (1-6) : 5
Hell, You back 6 stage.
(now you stay stage 41.)

choose number (1-6) : 6
Hell, You back 6 stage.
(now you stay stage 41.)

choose number (1-6) : 2
No hell and heaven.
(now you stay stage 43.)

choose number (1-6) : 1
Hell, You back 6 stage.
(now you stay stage 38.)

choose number (1-6) : 6
Hell, You back 6 stage.
(now you stay stage 38.)

choose number (1-6) : 5
No hell and heaven.
(now you stay stage 43.)

choose number (1-6) : 2
Heaven, You go to 3 stage.
(now you stay stage 48.)

choose number (1-6) : 2
>>> You win <<<
(now you stay stage 50.)

You choose 21 time.
```
