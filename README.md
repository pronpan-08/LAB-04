พรพรรณ เกิดรัตน์ 57030201 


#ใบงานที่ 4
เรื่อง การใช้งานคำสั่งเกี่ยวกับการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C#
##วัตถุประสงค์
1. เพื่อให้นักศึกษาบอกชื่อ method ที่ใช้ในการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C# ได้
2. เพื่อให้นักศึกษาสามารถใช้คำสั่งแสดงผลทางหน้าจอ เบื้องต้นได้

##ลำดับขั้นการทดลอง
###การเตรียมการก่อนการทดลอง
  * เปิดโปรแกรม Visual Studio 
  *  เลือก File >>New Project >> เลือก Console Application 
![P1](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P1.png)
  *  ช่อง Name ใส่ชื่อของ project (ในที่นี้คือ Lab4)
  *  ช่อง Location ใส่ชื่อ folder ที่เป็นที่ตั้งของ Project (ในที่นี้ สมมติเป็น E:\vslab)
  *  ช่อง Solution name ให้ใส่ชื่อ Solution โดยปกติก็ให้ปล่อยไว้อย่างนั้น 
  *  กดปุ่ม OK โปรแกรม Visual Studio จะสร้าง project ชื่อ “lab4”ภายใต้ solution “lab4” และไฟล์ lsb4.cs ซึ่งมี source code ดังรูป 

![P2](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P2.png)

ส่วนสำคัญของโปรแกรม lab4.cs  คือบรรทัดที่ 1 “using System” และเมธอด Main(string[] args)


 *  ให้ลบ source code ในบรรทัดที่ 2-5 ออกไปก่อน เนื่องจากเป็น assembly ที่ไม่จำเป็นต่อการทำงานของโปรแกรม 

## 1. การทดลองเมดธอด Console.Write()
* ให้เพิ่ม บรรทัดต่อไปนี้ลงไปในในเมธอด Main()
```csharp 
    Console.Write(“Hello”);
```
ดังปรากฏในบรรทัดที่ 9 ของรูปด้านล่าง 

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P3.png)
 
 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

####บันทึกผลการทดลอง

จากการทดลอง lab4 ทำการเปิดโปรกรม Visual Studio 2015 และทำตามขั้นตอนต่างๆในใบงานเปลี่ยนส่วนโค้ดที่ให้เปลี่ยนและกด Ctrl+F5 จะแสดง command line หรือหน้าต่างสีดำ แสดงคำ Hello

![](https://github.com/pronpan-08/LAB-04/blob/master/imgs/lab4-1joy.png?raw=true)
<hr>
<hr>
<hr>
<hr>
<hr>

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้    

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P4.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม
 * การรันแล้วทำให้หน้าจอ console ยังคงแสดงผลค้างอยู่นั้น ให้เลือกเมนู Debug -> Start Without Debugging (Ctrl+F5) มิฉะนั้น หน้าจอ console จะหายไปอย่างรวดเร็ว
<hr>
<hr>
<hr>
<hr>
<hr>
จากการทดลองทำการเพิ่มโค๊ตตามขั้นตอน เมื่อกด Ctrl+F5 อีกครั้งจะแสดงคำว่าHelloWorld ติดกัน

![](https://github.com/pronpan-08/LAB-04/blob/master/imgs/lab4-2joy.png?raw=true)

### คำถาม 4.1 

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย

ตอบ  ไม่เป็นอย่างที่คิดตอนแรกนึกว่าจะขึ้นคนละบันทัดแต่นี่ขึ้นติดกัน HelloWorld
<hr>
<hr>
<hr>
<hr>
<hr>


## 2. การทดลองเมดธอด Console.WriteLine()

แก้โปรแกรมในเมดธอด Main() ให้เป็นดังรูปต่อไปนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P5.png)

 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

บันทึกผลที่ได้จากการรันโปรแกรม

เมื่อทำการแก้โปรตามรูแล้วกด Ctrl+F5 จะแสดงคำว่า Hello แล้ว Enter บรรทัดลงมา 


![](https://github.com/pronpan-08/LAB-04/blob/master/imgs/lab4-3joy.png?raw=true)
<hr>
<hr>
<hr>
<hr>
<hr>

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P6.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม 
 
 
 เมื่อแก้ไขโปรแกรมตามรูป และกด Ctrl+F5 บรรทัดแรกจะแสดงคำว่า Hello และบรรทัดที่2 แสดงคำว่า World
 
 ![](https://github.com/pronpan-08/LAB-04/blob/master/imgs/lab4-4joy.png?raw=true)
<hr>
<hr>
<hr>
<hr>
<hr>

###คำถาม 4.2

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย

 ตอบ เป็นไปอย่างที่คิดคือ จะแสดง command line ที่แสดง บรรทัดแรกจะแสดงคำว่า Hello และบรรทัดที่2 แสดงคำว่า World
<hr>
<hr>
<hr>
<hr>
<hr>

### คำถาม 4.3 

จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()

ตอบ Console.Write() จะแสดง command line ที่แสดง คำตามที่เรากำหนด ดังเช่นการทดลองคือ Hello
    Console.WriteLine() จะแสดง command line ที่แสดง คำตามที่เรากำหนด ดังเช่นการทดลองคือ Hello แต่จะ enter บรรทัดลงมาหนึ่งบรรทัด
<hr>
<hr>
<hr>
<hr>
<hr>

##สรุปผลการทดลอง

   จากการทดลอง lab4 ทำการเปิดโปรกรม Visual Studio 2015 และทำตามขั้นตอนต่างๆในใบงานเปลี่ยนส่วนโค้ดที่ให้เปลี่ยนและกด Ctrl+F5 เมื่อใช้คำสั่งConsole.Write() จะแสดง command line ที่แสดง คำตามที่เรากำหนด ดังเช่นการทดลองคือ Hello แต่เมื่อใช้คำสั่ง Console.WriteLine() จะแสดง command line ที่แสดง คำตามที่เรากำหนด ดังเช่นการทดลองคือ Hello แต่จะ enter บรรทัดลงมาหนึ่งบรรทัด

<hr>
<hr>
<hr>
<hr>
<hr>

