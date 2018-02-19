เมื่อไหร่หนี้จะหมด?
จงเขียนโปรแกรมเพื่อรับจำนวนเต็มหนี้สินทั้งหมด ดอกเบี้ยที่จะต้องจ่าย จำนวนเงินที่ผ่อนคืนในแต่ละเดือน โดยแสดงผลเป็นจำนวนปีที่จะหมดหนี้
สำหรับดอกเบี้ยนั้น ให้รับข้อมูลเป็นร้อยละ ซึ่งไม่เกินร้อยละ 3 ต่อเดือน โดยคิดดอกเบี้ยทบต้น
คิดดอกเบี้ยแต่ละเดือนโดยใช้สูตร (วงเงินกู้*ร้อยละ)/12
สำหรับ input ที่ไม่ถูกต้อง ให้แสดงผลว่า “Invalid Input.” และให้ผู้ใช้ใส่เฉพาะค่านั้นใหม่อีกครั้ง

ตัวอย่าง input/output

Enter loan amount: 3000
Enter interest rate in percent: 0.03
Enter monthly payment: 500
It needs to take after 1 years.

Enter loan amount: 0
Invalid Input.
Enter loan amount: 12000
Enter interest rate in percent: 0
Enter monthly payment: -9
Invalid Input.
Enter monthly payment: 1000
It needs to take after 1 years.