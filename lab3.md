# การทดลองที่ 3 เรื่อง การเขียนโปรแกรมเอ้าพุทสัญญาณดิจิทัล
## วัตถุประสงค์
1.ศึกษาการทำงานของ relay 

2.ศึกษา output ของสัญญาณดิจิทัล

3.ศึกษาการเขียนโปรแกรม output สัญญาณดิจิทัล

## อุปกรณ์ที่ใช้

1.คอมพิวเตอร์

2.สาย USB

3.serial port

4.ไมโครคอนโทรลเลอร์ (ESP01)

5.relay

6.หลอดไฟ LED 

7.adapter 

## ศึกษาข้อมูลเบื้องต้น
https://www.youtube.com/watch?v=CCnN1WJsXQY

https://www.youtube.com/watch?v=6JnhaUILGuw

## วิธีการทำการทดลอง

1.นำ adapter ที่ต่ออยู่กับ LED ต่อเข้ากับ serial port แล้วจึงนำไมโครคอนโทรลเลอร์ต่อผ่าน adapter อีกที

![image](https://user-images.githubusercontent.com/80881680/112372159-03f13800-8d12-11eb-97db-4c7469de1e02.png)

2.เลือกตัวอย่างโปรแกรมที่ต้องการใช้ในที่นี้จะเลือกตัวอย่างที่ 3

  * พิมพ์ cd 03_Output-Port
  * พิมพ์ vi src/main.cpp

![image](https://user-images.githubusercontent.com/80881680/112372755-c50fb200-8d12-11eb-868e-a71988fc6bd9.png)

3.upload โปรแกรมเข้าไปที่ไมโครคอนโทรลเลอร์โดยในขณะที่รันจะกดปุ่มดำเพื่อให้ไมโครคอนโทรลเลอร์รับคำสั่งและกดปุ่มสีแดงเพื่อ reset

![image](https://user-images.githubusercontent.com/80881680/112373001-1324b580-8d13-11eb-98ab-aa1925fd4deb.png)

4.หลังจาก upload เรียบร้อยจะใช้คำสั่ง pio device monitor เพื่อดูผลลัพธ์ที่แสดงผลออกมา

![image](https://user-images.githubusercontent.com/80881680/112373109-2d5e9380-8d13-11eb-879e-6de8fe66bcc0.png)

5.หลังจากได้เขียนโปรแกรมเข้าไปในไมโครคอนโทรลเลอร์เรียบร้อยแล้ว จะนำไมโครคอนโทรเลอร์ที่ถูกเขียนโปรแกรมแล้วนั้นมาต่อเข้ากับ relay 

![image](https://user-images.githubusercontent.com/80881680/112373662-c9889a80-8d13-11eb-9fb6-a852b6d7fe1c.png)

6.นำแหล่งจ่ายไฟมาต่อเข้ากับ relay 

![image](https://user-images.githubusercontent.com/80881680/112373866-03f23780-8d14-11eb-8fbd-aec26c49e8e4.png)

## การบันทึกผลการทดลอง
  ก่อนต่อกับ relay 
    * เมื่อนับออกมาแล้วเป็นเลขคี่ หลอดไฟจะติด(ON)
    * เมื่อนับออกมาแล้วเป็นเลขคู่ หลอดไฟจะดับ (OFF)
   
  หลังต่อกับ relay 
    * relay จะสว่างและดับลงไปเรื่อยๆซึ่งการที่ relay มีลักษณะเช่นนี้นั้นเป็นเพราะโปรแกรมที่ได้เขียนลงไปในไมโครคอนโทรลเลอร์ซึ่ง relay จะสว่างเมื่อเป็น ON และจะดับลงเมื่อเป็น OFF เหมือนกับหลอดไฟ

## อภิปรายผลการทดลอง
  relay นั้นทำงาานสอดคล้องกับโปรแกรมที่ได้เขียนไว้ในไมโครคอนโทรลเลอร์โดยการสว่างและดับของ relay นั้นจะมีระยะเวลาห่างกัน 500ms ซึ่งเป็นตัวเลขที่ได้เขียนไว้ในโปรแกรม
  
## คำถามหลังการทดลอง
หากเปลี่ยนเวลาเป็น 1000ms จะเกิดอะไรขึ้น
  - relay จะสว่างและดับโดยมีระยะเวลาห่างกัน 1000ms


