# การทดลองที่ 5 เรื่อง การเขียนโปรแกรมเชื่อมต่อไวไฟและเว็บเซอร์เวอร์
## วัตถุประสงค์
1.เพื่อศึกษาการเขียนโปรแกรมเชื่อมต่อไวไฟและเว็บเซอร์เวอร์

## อุปกรณ์ที่ใช้
1.คอมพิวเตอร์

2.serial port

3.ไมโครคอนโทรลเลอร์ (ESP01)

4.สาย USB

## ศึกษาข้อมูลเบื้องต้น
https://www.youtube.com/watch?v=VX-QNQcO-b4

## วิธีการทำการทดลอง 
1.เลือกตัวอย่างโปรแกรมที่ต้องการใช้ในที่นี้จะเลือกตัวอย่างที่ 5

พิมพ์ cd 05_Wifi-Web-Server
พิมพ์ vi src/main.cpp

![image](https://user-images.githubusercontent.com/80881680/112382990-23db2880-8d1f-11eb-821b-70d99c857baa.png)

![image](https://user-images.githubusercontent.com/80881680/112383024-2d649080-8d1f-11eb-8e21-255bb2257656.png)

2.upload โปรแกรมในขณะที่อัพโหลดนำไมโครคอนโทรลเลอร์ไปต่อโดยในขณะที่รันจะกดปุ่มดำเพื่อให้ไมโครคอนโทรลเลอร์รับคำสั่งและกดปุ่มสีแดงเพื่อ reset

3.หลังจาก upload เรียบร้อยจะใช้คำสั่ง pio device monitor เพื่อดูผลลัพธ์ที่แสดงผลออกมาโดยผลลัพธ์ที่แสดงออกมานั้นจะเป็น ip address แล้วจึงนำ ip address ไปทดสอบที่ browser

![image](https://user-images.githubusercontent.com/80881680/112383595-e88d2980-8d1f-11eb-9f77-c775fe5cf1d2.png)

## การบันทึกผลการทดลอง
  ผลลัพธ์ที่แสดงออกมานั้นจะเป็น Hello 1 แล้วนับไปเรื่อยๆโดยจะเปลี่ยน cnt จะเปลี่ยนตัวแปรไปเรื่อยๆ 
  
## อภิปรายผลการทดลอง
  จากการทดลองสามารถทดสอบโปรแกรมได้โดยการนำ ip address ไปใส่ที่ browser เพื่อทดสอบโปรแกรมได้
  
## คำถามหลังการทดลอง
  อะไรที่สามารถเชื่อมต่อกับ wifi ได้นอกจาก password 
    * ssid


