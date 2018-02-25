# -Gunner- #

โจทย์ให้เขียนโปรแกรม รับคะแนนจากเกมส์ เพื่อนำมาประมวลอันดับ Ranking และ รางวัลพิเศษ ต่างๆ ภายในเกมที่ได้รับ จากการฆ่าสัตว์ประหลาด หรือ คน ให้บอกจำนวนการฆ่า ในแต่ละระดับเลเวลเพื่อนำมา คำนวน score ผู้เล่น

## ข้อมูลนำเข้า ##

บรรทัด ที่ 1 รับค่าระดับความยาก

บรรทัด ที่ 2 รับจำนวนการฆ๋า monster

บรรทัด ที่ 3 รับจำนวนการฆ่า human

## ข้อมูลออก ##

บอก score ของผู้เล่น

บอก Ranking ของผู้เล่น

บอก point พิเศษ ที่ผู้เล่นได้รับ

## หมายเหตุ ##


1.  การฆ่า จะได้คะแนน ตามระดับเลเวล โดยที่ เลเวล 1 monster 	จะอย่ที่ 200 point | human จะอยู่ที่ 50 point
 -โดย หากเลเวล เพิ่มขึ้น 1 จะเพิ่ม คะแนนที่ได้รับอย่างละ 50 point

2.  จะได้รับ รางวัลพิเศษ จากการฆ่า monster ที่ 20 point human 5 point โดย หากเลเวลเพิ่มขึ้น 1 จเพิ่ม รางวัลที่ได้รับ 10 point

3.  เลเวล ไม่สามารถเกิน 3 ระดับ

## Test case ##
```
Enter your Level: 1
Score monster kill: 2
Score human kill: 4
Your score is: 600
--- Your ranking is Silver ---
---| Congratulation your get reward!!!|---
Your get 80 point for free
Thanks for play
```

```
Enter your level: 4
Level it can't be more than 3
```

```
Enter your level: 0
Please select level 1-3
```
