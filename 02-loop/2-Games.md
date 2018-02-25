# 2 Games
ทำการรับตัวอักษรแรกของชื่อผู้เล่น และเลือกเกมที่ต้องการเล่น โดยทุกครั้งที่เลือกเกมจะขึ้นข้อความ "Welcome to Game#เลขเกมที่ผู้เล่นเลือก" และเมื่อจบเกมจะจบด้วยประโยค "Thanks for playing!"เสมอ
* เกมที่1
    - ทำการเดาเลขที่มีค่าตั้งแต่0-80 โดยมี target = 60
    - เมื่อทายถูกจะขึ้นตัวอักษรตัวแรกของผู้เล่นและแสดงข้อความว่าทายถูกแล้ว
    - ถ้าทายผิดเกมจะแสดงข้อความว่าเราผิดและจะกลับมารับค่าคำตอบใหม่อีกเรื่อยๆจนกว่าผู้เล่นจะทายถูก
* เกมที่2
    - ผู้เล่นต้องเติมคำตอบของสมการที่กำหนดให้โดยให้ตอบเป็นจำนวนเต็มบวก(คำตอบของสมการมีหลายคำตอบ)ให้ตอบเพียงคำตอบเดียว
    - เมื่อผู้เล่นทายถูกจะแสดงว่าผู้เล่นชนะ
    - หากตอบผิดเกมจะแสดงข้อความว่าเราแพ้และจะให้กลับมาเติมคำใหม่เรื่อยๆจนกว่าจะถูก
    # Input
    * บรรทัดแรกรับตัวอักษรนำหน้าชื่อผู้เล่น1ตัว
    * บรรทัดสองรับค่าเลขของเกมที่ต้องการเล่น
    * ใส่คำตอบของคำถามจากเกมที่เลือก
    # Output
    * ถ้าทายผิดเกม1จะแสดงข้อความว่า "Your guess is wrong."
    * ถ้าทายผิดเกม2จะแสดงข้อความว่า "Answer is wrong."
    * กรณีทายถูกแสดงตัวอักษรนำหน้าชื่อที่Input ตามด้วย "is win!"
    * ทุกครั้งที่เล่นเกมชนะจะขึ้นข้อความว่า "Thanks for playing!"

    # ตัวอย่างInput/Output 1
    Enter your First Character name: b\
    Select game number[1,2]: 1\
    Welcome to Game#1\
    Guess the number(0-80)? 0\
    Your guess is wrong.\
    Guess the number(0-80)? 25\
    Your guess is wrong.\
    Guess the number(0-80)? 50\
    Your guess is wrong.\
    Guess the number(0-80)?\
    (จะรับค่าจนกว่าจะเติมคำตอบที่ถูกต้อง)

    # ตัวอย่างInput/Output 2
    Enter your First Character name: b\
    Select game number[1,2]: 1\
    Welcome to Game#1\
    Guess the number(0-80)? 60\
    b is win!\
    Thanks for playing!

    # ตัวอย่างInput/Output 3
    Enter your First Character name: b\
    Select game number[1,2]: 2\
    Welcome to Game#2\
    Answer the interger positive number of function!!!\
    (3*(x**3)) + (2(x**2)) - (12*x) - 8 = 0\
    Answer: 5\
    Answer is wrong.\
    Answer: 1\
    Answer is wrong.\
    Answer: 0\
    Answer is wrong.\
    Answer: 2\
    b is win!\
    Thanks for playing!
