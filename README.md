# Auto Suggest Ahead

ไม่รู้จะเรียกอะไร บ้างก็เรียก `autocomplete` แต่บางคนเรียก `suggestion` ก็มี ส่วน `type ahead` ก็มา

สรุปว่า workshop นี้จะทำตัวช่วยค้นหาสถานที่ในประเทศไทย โดยใช้ฐานข้อมูลจาก

https://github.com/earthchie/jquery.Thailand.js

ต้องขอขอบคุณด้วยนะครับ ลองไปดูชิ้นงานต้นฉบับได้ที่

https://earthchie.github.io/jquery.Thailand.js/

แต่เนื่องจากเราเป็นคนหวานๆ เราจะใช้ Vanilla JS ในการทำนะจ๊ะ 💁🏻‍♀️

ไฟล์ `index.html` ที่เตรียมไว้ให้ เมื่อ load ขึ้นมาก็จะมี `cities` พร้อมให้ใช้แล้ว

ก่อนเข้า workshop สามารถลองทำการรับค่าจาก `input` มาทำ `array.filter()` ก่อนได้เลยยย

# Note หลังเรียน 
## วิธีการดึงข้อมูลจาก JSON มา สร้างเป็น excel
 * 1. let keys=Object.keys(cities[0])
 * 2. keys;
 * 3. keys.map(k=> cities[3][k]);
 * 4. keys.join();
 * 5. cities.reduce((sum,c)=>{
	  return sum + keys.map(k=> c[k]+"\n")
   }, keys.join() +"\n");
